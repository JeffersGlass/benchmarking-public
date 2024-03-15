# Results vs. base

- fork: brandtbucher
- ref: justin_continue
- machine: linux-x86_64
- commit hash: 9e86002
- commit date: 2024-02-13
- overall geometric mean: 1.01x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 276 ms                                                                 | 273 ms: 1.01x faster                                                    |
| chameleon      | 6.89 ms                                                                | 6.74 ms: 1.02x faster                                                   |
| docutils       | 2.64 sec                                                               | 2.62 sec: 1.01x faster                                                  |
| tornado_http   | 97.2 ms                                                                | 96.7 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_memoization_tg  | 594 ms                                                                 | 573 ms: 1.04x faster                                                    |
| async_tree_io              | 1.20 sec                                                               | 1.17 sec: 1.02x faster                                                  |
| async_tree_io_tg           | 1.21 sec                                                               | 1.19 sec: 1.02x faster                                                  |
| async_tree_none_tg         | 457 ms                                                                 | 448 ms: 1.02x faster                                                    |
| async_tree_cpu_io_mixed    | 723 ms                                                                 | 708 ms: 1.02x faster                                                    |
| async_tree_memoization     | 572 ms                                                                 | 563 ms: 1.02x faster                                                    |
| async_tree_cpu_io_mixed_tg | 732 ms                                                                 | 720 ms: 1.02x faster                                                    |
| Geometric mean             | (ref)                                                                  | 1.02x faster                                                            |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| nbody          | 102 ms                                                                 | 99.1 ms: 1.03x faster                                                   |
| float          | 86.6 ms                                                                | 84.2 ms: 1.03x faster                                                   |
| pidigits       | 188 ms                                                                 | 187 ms: 1.00x faster                                                    |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                                 | 136 ms: 1.03x faster                                                    |
| regex_v8       | 25.4 ms                                                                | 25.6 ms: 1.01x slower                                                   |
| regex_effbot   | 3.61 ms                                                                | 3.68 ms: 1.02x slower                                                   |
| regex_dna      | 219 ms                                                                 | 224 ms: 1.02x slower                                                    |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| tomli_loads          | 2.20 sec                                                               | 2.14 sec: 1.03x faster                                                  |
| pickle_pure_python   | 299 us                                                                 | 293 us: 1.02x faster                                                    |
| pickle               | 11.6 us                                                                | 11.4 us: 1.02x faster                                                   |
| xml_etree_generate   | 86.1 ms                                                                | 84.8 ms: 1.02x faster                                                   |
| xml_etree_iterparse  | 108 ms                                                                 | 106 ms: 1.01x faster                                                    |
| xml_etree_process    | 58.0 ms                                                                | 57.3 ms: 1.01x faster                                                   |
| unpickle_pure_python | 226 us                                                                 | 223 us: 1.01x faster                                                    |
| unpickle_list        | 4.85 us                                                                | 5.04 us: 1.04x slower                                                   |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                            |

Benchmark hidden because not significant (6): json_dumps, xml_etree_parse, pickle_dict, pickle_list, json_loads, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|------------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 10.3 ms                                                                | 10.2 ms: 1.01x faster                                                   |
| python_startup_no_site | 8.87 ms                                                                | 8.83 ms: 1.00x faster                                                   |
| Geometric mean         | (ref)                                                                  | 1.01x faster                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|-----------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 12.5 ms                                                                | 12.0 ms: 1.04x faster                                                   |

All benchmarks:
===============

| Benchmark                  | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| gc_traversal               | 3.85 ms                                                                | 3.47 ms: 1.11x faster                                                   |
| mdp                        | 2.78 sec                                                               | 2.57 sec: 1.08x faster                                                  |
| hexiom                     | 8.00 ms                                                                | 7.52 ms: 1.06x faster                                                   |
| pprint_pformat             | 1.64 sec                                                               | 1.55 sec: 1.06x faster                                                  |
| pprint_safe_repr           | 788 ms                                                                 | 752 ms: 1.05x faster                                                    |
| mako                       | 12.5 ms                                                                | 12.0 ms: 1.04x faster                                                   |
| chaos                      | 70.5 ms                                                                | 67.8 ms: 1.04x faster                                                   |
| spectral_norm              | 136 ms                                                                 | 131 ms: 1.04x faster                                                    |
| async_tree_memoization_tg  | 594 ms                                                                 | 573 ms: 1.04x faster                                                    |
| regex_compile              | 141 ms                                                                 | 136 ms: 1.03x faster                                                    |
| typing_runtime_protocols   | 112 us                                                                 | 108 us: 1.03x faster                                                    |
| nbody                      | 102 ms                                                                 | 99.1 ms: 1.03x faster                                                   |
| comprehensions             | 19.3 us                                                                | 18.7 us: 1.03x faster                                                   |
| float                      | 86.6 ms                                                                | 84.2 ms: 1.03x faster                                                   |
| deepcopy_memo              | 38.4 us                                                                | 37.3 us: 1.03x faster                                                   |
| nqueens                    | 90.3 ms                                                                | 87.8 ms: 1.03x faster                                                   |
| tomli_loads                | 2.20 sec                                                               | 2.14 sec: 1.03x faster                                                  |
| coverage                   | 96.5 ms                                                                | 94.0 ms: 1.03x faster                                                   |
| richards_super             | 51.9 ms                                                                | 50.6 ms: 1.03x faster                                                   |
| richards                   | 45.9 ms                                                                | 44.8 ms: 1.03x faster                                                   |
| create_gc_cycles           | 1.50 ms                                                                | 1.46 ms: 1.02x faster                                                   |
| async_tree_io              | 1.20 sec                                                               | 1.17 sec: 1.02x faster                                                  |
| sqlglot_optimize           | 56.0 ms                                                                | 54.8 ms: 1.02x faster                                                   |
| scimark_monte_carlo        | 74.0 ms                                                                | 72.4 ms: 1.02x faster                                                   |
| chameleon                  | 6.89 ms                                                                | 6.74 ms: 1.02x faster                                                   |
| async_tree_io_tg           | 1.21 sec                                                               | 1.19 sec: 1.02x faster                                                  |
| async_tree_none_tg         | 457 ms                                                                 | 448 ms: 1.02x faster                                                    |
| async_tree_cpu_io_mixed    | 723 ms                                                                 | 708 ms: 1.02x faster                                                    |
| sympy_sum                  | 160 ms                                                                 | 157 ms: 1.02x faster                                                    |
| sympy_expand               | 480 ms                                                                 | 471 ms: 1.02x faster                                                    |
| deepcopy_reduce            | 3.08 us                                                                | 3.03 us: 1.02x faster                                                   |
| pickle_pure_python         | 299 us                                                                 | 293 us: 1.02x faster                                                    |
| pickle                     | 11.6 us                                                                | 11.4 us: 1.02x faster                                                   |
| raytrace                   | 280 ms                                                                 | 276 ms: 1.02x faster                                                    |
| logging_silent             | 101 ns                                                                 | 99.4 ns: 1.02x faster                                                   |
| sympy_str                  | 284 ms                                                                 | 279 ms: 1.02x faster                                                    |
| deepcopy                   | 346 us                                                                 | 340 us: 1.02x faster                                                    |
| dulwich_log                | 68.4 ms                                                                | 67.3 ms: 1.02x faster                                                   |
| sqlglot_normalize          | 109 ms                                                                 | 108 ms: 1.02x faster                                                    |
| async_tree_memoization     | 572 ms                                                                 | 563 ms: 1.02x faster                                                    |
| deltablue                  | 3.38 ms                                                                | 3.33 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed_tg | 732 ms                                                                 | 720 ms: 1.02x faster                                                    |
| xml_etree_generate         | 86.1 ms                                                                | 84.8 ms: 1.02x faster                                                   |
| sqlglot_parse              | 1.29 ms                                                                | 1.27 ms: 1.02x faster                                                   |
| xml_etree_iterparse        | 108 ms                                                                 | 106 ms: 1.01x faster                                                    |
| xml_etree_process          | 58.0 ms                                                                | 57.3 ms: 1.01x faster                                                   |
| unpickle_pure_python       | 226 us                                                                 | 223 us: 1.01x faster                                                    |
| sqlglot_transpile          | 1.62 ms                                                                | 1.60 ms: 1.01x faster                                                   |
| dask                       | 366 ms                                                                 | 361 ms: 1.01x faster                                                    |
| go                         | 147 ms                                                                 | 146 ms: 1.01x faster                                                    |
| sqlite_synth               | 2.81 us                                                                | 2.78 us: 1.01x faster                                                   |
| sympy_integrate            | 20.9 ms                                                                | 20.7 ms: 1.01x faster                                                   |
| telco                      | 8.61 ms                                                                | 8.52 ms: 1.01x faster                                                   |
| 2to3                       | 276 ms                                                                 | 273 ms: 1.01x faster                                                    |
| bench_thread_pool          | 843 us                                                                 | 836 us: 1.01x faster                                                    |
| docutils                   | 2.64 sec                                                               | 2.62 sec: 1.01x faster                                                  |
| python_startup             | 10.3 ms                                                                | 10.2 ms: 1.01x faster                                                   |
| tornado_http               | 97.2 ms                                                                | 96.7 ms: 1.01x faster                                                   |
| meteor_contest             | 110 ms                                                                 | 110 ms: 1.00x faster                                                    |
| asyncio_tcp_ssl            | 1.81 sec                                                               | 1.80 sec: 1.00x faster                                                  |
| python_startup_no_site     | 8.87 ms                                                                | 8.83 ms: 1.00x faster                                                   |
| asyncio_tcp                | 494 ms                                                                 | 492 ms: 1.00x faster                                                    |
| pidigits                   | 188 ms                                                                 | 187 ms: 1.00x faster                                                    |
| async_generators           | 460 ms                                                                 | 461 ms: 1.00x slower                                                    |
| regex_v8                   | 25.4 ms                                                                | 25.6 ms: 1.01x slower                                                   |
| logging_simple             | 5.67 us                                                                | 5.71 us: 1.01x slower                                                   |
| generators                 | 29.2 ms                                                                | 29.6 ms: 1.02x slower                                                   |
| regex_effbot               | 3.61 ms                                                                | 3.68 ms: 1.02x slower                                                   |
| regex_dna                  | 219 ms                                                                 | 224 ms: 1.02x slower                                                    |
| pathlib                    | 18.1 ms                                                                | 18.5 ms: 1.02x slower                                                   |
| pycparser                  | 1.17 sec                                                               | 1.21 sec: 1.03x slower                                                  |
| unpack_sequence            | 48.3 ns                                                                | 50.2 ns: 1.04x slower                                                   |
| unpickle_list              | 4.85 us                                                                | 5.04 us: 1.04x slower                                                   |
| scimark_sor                | 119 ms                                                                 | 124 ms: 1.05x slower                                                    |
| Geometric mean             | (ref)                                                                  | 1.01x faster                                                            |

Benchmark hidden because not significant (19): async_tree_none, json, mypy2, fannkuch, scimark_fft, crypto_pyaes, coroutines, json_dumps, xml_etree_parse, pickle_dict, pickle_list, pyflate, scimark_sparse_mat_mult, json_loads, bench_mp_pool, asyncio_websockets, unpickle, scimark_lu, logging_format


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x