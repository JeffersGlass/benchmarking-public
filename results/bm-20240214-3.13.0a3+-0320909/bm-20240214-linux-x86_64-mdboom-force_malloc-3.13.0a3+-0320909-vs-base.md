# Results vs. base

- fork: mdboom
- ref: force_malloc
- machine: linux-x86_64
- commit hash: 0320909
- commit date: 2024-02-14
- overall geometric mean: 1.00x faster
- HPT reliability: 98.87%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| chameleon      | 6.77 ms                                                                | 6.82 ms: 1.01x slower                                          |
| docutils       | 2.60 sec                                                               | 2.59 sec: 1.00x faster                                         |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                   |

Benchmark hidden because not significant (2): 2to3, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none_tg         | 441 ms                                                                 | 427 ms: 1.03x faster                                           |
| async_tree_io              | 1.18 sec                                                               | 1.15 sec: 1.02x faster                                         |
| async_tree_memoization_tg  | 569 ms                                                                 | 557 ms: 1.02x faster                                           |
| async_tree_cpu_io_mixed_tg | 717 ms                                                                 | 703 ms: 1.02x faster                                           |
| async_tree_io_tg           | 1.18 sec                                                               | 1.17 sec: 1.01x faster                                         |
| Geometric mean             | (ref)                                                                  | 1.02x faster                                                   |

Benchmark hidden because not significant (3): async_tree_none, async_tree_cpu_io_mixed, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| float          | 79.3 ms                                                                | 76.2 ms: 1.04x faster                                          |
| pidigits       | 188 ms                                                                 | 187 ms: 1.00x faster                                           |
| nbody          | 88.2 ms                                                                | 91.9 ms: 1.04x slower                                          |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 128 ms                                                                 | 127 ms: 1.01x faster                                           |
| regex_dna      | 217 ms                                                                 | 220 ms: 1.01x slower                                           |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                   |

Benchmark hidden because not significant (2): regex_effbot, regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| unpickle             | 16.6 us                                                                | 15.4 us: 1.07x faster                                          |
| xml_etree_parse      | 159 ms                                                                 | 156 ms: 1.02x faster                                           |
| pickle_list          | 5.22 us                                                                | 5.13 us: 1.02x faster                                          |
| pickle               | 12.0 us                                                                | 11.8 us: 1.02x faster                                          |
| unpickle_list        | 4.97 us                                                                | 4.89 us: 1.02x faster                                          |
| xml_etree_generate   | 85.3 ms                                                                | 84.5 ms: 1.01x faster                                          |
| pickle_dict          | 34.9 us                                                                | 34.7 us: 1.01x faster                                          |
| json_dumps           | 10.4 ms                                                                | 10.4 ms: 1.01x slower                                          |
| unpickle_pure_python | 211 us                                                                 | 212 us: 1.01x slower                                           |
| json_loads           | 27.3 us                                                                | 27.7 us: 1.01x slower                                          |
| tomli_loads          | 2.08 sec                                                               | 2.13 sec: 1.02x slower                                         |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                   |

Benchmark hidden because not significant (3): xml_etree_process, pickle_pure_python, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 10.0 ms                                                                | 10.1 ms: 1.00x slower                                          |
| python_startup_no_site | 8.67 ms                                                                | 8.70 ms: 1.00x slower                                          |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 11.1 ms                                                                | 11.1 ms: 1.00x slower                                          |

All benchmarks:
===============

| Benchmark                  | bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| unpickle                   | 16.6 us                                                                | 15.4 us: 1.07x faster                                          |
| coroutines                 | 22.7 ms                                                                | 21.5 ms: 1.05x faster                                          |
| float                      | 79.3 ms                                                                | 76.2 ms: 1.04x faster                                          |
| unpack_sequence            | 51.7 ns                                                                | 49.8 ns: 1.04x faster                                          |
| async_tree_none_tg         | 441 ms                                                                 | 427 ms: 1.03x faster                                           |
| logging_silent             | 97.8 ns                                                                | 95.2 ns: 1.03x faster                                          |
| async_tree_io              | 1.18 sec                                                               | 1.15 sec: 1.02x faster                                         |
| bench_thread_pool          | 817 us                                                                 | 798 us: 1.02x faster                                           |
| xml_etree_parse            | 159 ms                                                                 | 156 ms: 1.02x faster                                           |
| async_tree_memoization_tg  | 569 ms                                                                 | 557 ms: 1.02x faster                                           |
| async_tree_cpu_io_mixed_tg | 717 ms                                                                 | 703 ms: 1.02x faster                                           |
| deepcopy_reduce            | 3.01 us                                                                | 2.95 us: 1.02x faster                                          |
| pyflate                    | 456 ms                                                                 | 447 ms: 1.02x faster                                           |
| pickle_list                | 5.22 us                                                                | 5.13 us: 1.02x faster                                          |
| pickle                     | 12.0 us                                                                | 11.8 us: 1.02x faster                                          |
| unpickle_list              | 4.97 us                                                                | 4.89 us: 1.02x faster                                          |
| logging_format             | 6.19 us                                                                | 6.09 us: 1.02x faster                                          |
| async_tree_io_tg           | 1.18 sec                                                               | 1.17 sec: 1.01x faster                                         |
| coverage                   | 97.1 ms                                                                | 95.9 ms: 1.01x faster                                          |
| spectral_norm              | 110 ms                                                                 | 108 ms: 1.01x faster                                           |
| richards_super             | 53.3 ms                                                                | 52.7 ms: 1.01x faster                                          |
| deepcopy_memo              | 37.5 us                                                                | 37.1 us: 1.01x faster                                          |
| generators                 | 29.8 ms                                                                | 29.5 ms: 1.01x faster                                          |
| logging_simple             | 5.61 us                                                                | 5.56 us: 1.01x faster                                          |
| xml_etree_generate         | 85.3 ms                                                                | 84.5 ms: 1.01x faster                                          |
| pathlib                    | 18.2 ms                                                                | 18.0 ms: 1.01x faster                                          |
| scimark_lu                 | 112 ms                                                                 | 111 ms: 1.01x faster                                           |
| comprehensions             | 16.0 us                                                                | 15.9 us: 1.01x faster                                          |
| regex_compile              | 128 ms                                                                 | 127 ms: 1.01x faster                                           |
| crypto_pyaes               | 71.1 ms                                                                | 70.6 ms: 1.01x faster                                          |
| sqlglot_normalize          | 106 ms                                                                 | 105 ms: 1.01x faster                                           |
| pickle_dict                | 34.9 us                                                                | 34.7 us: 1.01x faster                                          |
| go                         | 136 ms                                                                 | 135 ms: 1.01x faster                                           |
| asyncio_tcp                | 487 ms                                                                 | 484 ms: 1.01x faster                                           |
| sqlglot_optimize           | 53.5 ms                                                                | 53.2 ms: 1.00x faster                                          |
| scimark_fft                | 355 ms                                                                 | 354 ms: 1.00x faster                                           |
| mdp                        | 2.52 sec                                                               | 2.51 sec: 1.00x faster                                         |
| docutils                   | 2.60 sec                                                               | 2.59 sec: 1.00x faster                                         |
| pidigits                   | 188 ms                                                                 | 187 ms: 1.00x faster                                           |
| asyncio_tcp_ssl            | 1.79 sec                                                               | 1.79 sec: 1.00x faster                                         |
| dulwich_log                | 65.4 ms                                                                | 65.2 ms: 1.00x faster                                          |
| sympy_integrate            | 19.3 ms                                                                | 19.4 ms: 1.00x slower                                          |
| python_startup             | 10.0 ms                                                                | 10.1 ms: 1.00x slower                                          |
| sympy_sum                  | 147 ms                                                                 | 148 ms: 1.00x slower                                           |
| create_gc_cycles           | 1.46 ms                                                                | 1.46 ms: 1.00x slower                                          |
| mako                       | 11.1 ms                                                                | 11.1 ms: 1.00x slower                                          |
| python_startup_no_site     | 8.67 ms                                                                | 8.70 ms: 1.00x slower                                          |
| sqlglot_transpile          | 1.55 ms                                                                | 1.56 ms: 1.00x slower                                          |
| json_dumps                 | 10.4 ms                                                                | 10.4 ms: 1.01x slower                                          |
| chameleon                  | 6.77 ms                                                                | 6.82 ms: 1.01x slower                                          |
| async_generators           | 439 ms                                                                 | 442 ms: 1.01x slower                                           |
| sqlglot_parse              | 1.24 ms                                                                | 1.25 ms: 1.01x slower                                          |
| scimark_sparse_mat_mult    | 4.62 ms                                                                | 4.66 ms: 1.01x slower                                          |
| fannkuch                   | 378 ms                                                                 | 381 ms: 1.01x slower                                           |
| unpickle_pure_python       | 211 us                                                                 | 212 us: 1.01x slower                                           |
| json                       | 5.03 ms                                                                | 5.08 ms: 1.01x slower                                          |
| meteor_contest             | 106 ms                                                                 | 107 ms: 1.01x slower                                           |
| deltablue                  | 3.13 ms                                                                | 3.16 ms: 1.01x slower                                          |
| pprint_safe_repr           | 724 ms                                                                 | 732 ms: 1.01x slower                                           |
| pprint_pformat             | 1.47 sec                                                               | 1.49 sec: 1.01x slower                                         |
| hexiom                     | 5.97 ms                                                                | 6.04 ms: 1.01x slower                                          |
| regex_dna                  | 217 ms                                                                 | 220 ms: 1.01x slower                                           |
| json_loads                 | 27.3 us                                                                | 27.7 us: 1.01x slower                                          |
| pycparser                  | 1.14 sec                                                               | 1.16 sec: 1.02x slower                                         |
| tomli_loads                | 2.08 sec                                                               | 2.13 sec: 1.02x slower                                         |
| chaos                      | 58.1 ms                                                                | 59.5 ms: 1.02x slower                                          |
| nqueens                    | 77.9 ms                                                                | 80.6 ms: 1.03x slower                                          |
| nbody                      | 88.2 ms                                                                | 91.9 ms: 1.04x slower                                          |
| gc_traversal               | 3.46 ms                                                                | 3.69 ms: 1.07x slower                                          |
| Geometric mean             | (ref)                                                                  | 1.00x faster                                                   |

Benchmark hidden because not significant (24): async_tree_none, async_tree_cpu_io_mixed, async_tree_memoization, sympy_str, telco, typing_runtime_protocols, mypy2, dask, deepcopy, xml_etree_process, pickle_pure_python, richards, scimark_sor, xml_etree_iterparse, asyncio_websockets, regex_effbot, sympy_expand, sqlite_synth, scimark_monte_carlo, raytrace, bench_mp_pool, 2to3, regex_v8, tornado_http


# HPT report

- Reliability score: 98.87% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x