# Results vs. base

- fork: mdboom
- ref: force_mimalloc
- machine: linux-x86_64
- commit hash: f8250a4
- commit date: 2024-02-14
- overall geometric mean: 1.00x slower
- HPT reliability: 59.02%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 261 ms                                                                 | 258 ms: 1.01x faster                                             |
| chameleon      | 6.77 ms                                                                | 6.72 ms: 1.01x faster                                            |
| docutils       | 2.60 sec                                                               | 2.66 sec: 1.02x slower                                           |
| tornado_http   | 94.5 ms                                                                | 91.7 ms: 1.03x faster                                            |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 717 ms                                                                 | 771 ms: 1.07x slower                                             |
| async_tree_cpu_io_mixed    | 705 ms                                                                 | 763 ms: 1.08x slower                                             |
| async_tree_none_tg         | 441 ms                                                                 | 481 ms: 1.09x slower                                             |
| async_tree_none            | 432 ms                                                                 | 473 ms: 1.10x slower                                             |
| async_tree_memoization_tg  | 569 ms                                                                 | 628 ms: 1.10x slower                                             |
| async_tree_memoization     | 558 ms                                                                 | 628 ms: 1.13x slower                                             |
| async_tree_io_tg           | 1.18 sec                                                               | 1.34 sec: 1.14x slower                                           |
| async_tree_io              | 1.18 sec                                                               | 1.34 sec: 1.14x slower                                           |
| Geometric mean             | (ref)                                                                  | 1.11x slower                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------:|
| pidigits       | 188 ms                                                                 | 181 ms: 1.03x faster                                             |
| float          | 79.3 ms                                                                | 80.0 ms: 1.01x slower                                            |
| nbody          | 88.2 ms                                                                | 90.1 ms: 1.02x slower                                            |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_effbot   | 3.67 ms                                                                | 3.50 ms: 1.05x faster                                            |
| regex_v8       | 25.1 ms                                                                | 24.5 ms: 1.03x faster                                            |
| regex_compile  | 128 ms                                                                 | 126 ms: 1.02x faster                                             |
| regex_dna      | 217 ms                                                                 | 218 ms: 1.00x slower                                             |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------:|
| pickle               | 12.0 us                                                                | 11.5 us: 1.04x faster                                            |
| xml_etree_parse      | 159 ms                                                                 | 155 ms: 1.03x faster                                             |
| pickle_list          | 5.22 us                                                                | 5.11 us: 1.02x faster                                            |
| json_dumps           | 10.4 ms                                                                | 10.2 ms: 1.02x faster                                            |
| xml_etree_generate   | 85.3 ms                                                                | 84.1 ms: 1.01x faster                                            |
| xml_etree_iterparse  | 104 ms                                                                 | 103 ms: 1.01x faster                                             |
| unpickle_list        | 4.97 us                                                                | 4.92 us: 1.01x faster                                            |
| pickle_dict          | 34.9 us                                                                | 35.0 us: 1.00x slower                                            |
| xml_etree_process    | 58.0 ms                                                                | 58.5 ms: 1.01x slower                                            |
| unpickle_pure_python | 211 us                                                                 | 213 us: 1.01x slower                                             |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                     |

Benchmark hidden because not significant (4): unpickle, json_loads, tomli_loads, pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 10.0 ms                                                                | 10.1 ms: 1.00x slower                                            |
| python_startup_no_site | 8.67 ms                                                                | 8.70 ms: 1.00x slower                                            |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|-----------|:----------------------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 11.1 ms                                                                | 10.2 ms: 1.09x faster                                            |

All benchmarks:
===============

| Benchmark                  | bm-20240214-linux-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------:|
| unpack_sequence            | 51.7 ns                                                                | 40.8 ns: 1.27x faster                                            |
| mako                       | 11.1 ms                                                                | 10.2 ms: 1.09x faster                                            |
| spectral_norm              | 110 ms                                                                 | 101 ms: 1.08x faster                                             |
| coroutines                 | 22.7 ms                                                                | 21.5 ms: 1.05x faster                                            |
| pathlib                    | 18.2 ms                                                                | 17.3 ms: 1.05x faster                                            |
| regex_effbot               | 3.67 ms                                                                | 3.50 ms: 1.05x faster                                            |
| pickle                     | 12.0 us                                                                | 11.5 us: 1.04x faster                                            |
| sqlglot_normalize          | 106 ms                                                                 | 102 ms: 1.04x faster                                             |
| pyflate                    | 456 ms                                                                 | 438 ms: 1.04x faster                                             |
| sqlglot_optimize           | 53.5 ms                                                                | 51.5 ms: 1.04x faster                                            |
| pidigits                   | 188 ms                                                                 | 181 ms: 1.03x faster                                             |
| dulwich_log                | 65.4 ms                                                                | 63.4 ms: 1.03x faster                                            |
| sqlite_synth               | 2.81 us                                                                | 2.72 us: 1.03x faster                                            |
| tornado_http               | 94.5 ms                                                                | 91.7 ms: 1.03x faster                                            |
| generators                 | 29.8 ms                                                                | 29.0 ms: 1.03x faster                                            |
| sympy_str                  | 268 ms                                                                 | 260 ms: 1.03x faster                                             |
| deepcopy_memo              | 37.5 us                                                                | 36.5 us: 1.03x faster                                            |
| telco                      | 8.41 ms                                                                | 8.18 ms: 1.03x faster                                            |
| pycparser                  | 1.14 sec                                                               | 1.10 sec: 1.03x faster                                           |
| xml_etree_parse            | 159 ms                                                                 | 155 ms: 1.03x faster                                             |
| regex_v8                   | 25.1 ms                                                                | 24.5 ms: 1.03x faster                                            |
| pickle_list                | 5.22 us                                                                | 5.11 us: 1.02x faster                                            |
| json_dumps                 | 10.4 ms                                                                | 10.2 ms: 1.02x faster                                            |
| pprint_pformat             | 1.47 sec                                                               | 1.44 sec: 1.02x faster                                           |
| deepcopy                   | 339 us                                                                 | 332 us: 1.02x faster                                             |
| pprint_safe_repr           | 724 ms                                                                 | 710 ms: 1.02x faster                                             |
| regex_compile              | 128 ms                                                                 | 126 ms: 1.02x faster                                             |
| coverage                   | 97.1 ms                                                                | 95.5 ms: 1.02x faster                                            |
| sympy_sum                  | 147 ms                                                                 | 145 ms: 1.02x faster                                             |
| sqlglot_transpile          | 1.55 ms                                                                | 1.52 ms: 1.02x faster                                            |
| asyncio_websockets         | 551 ms                                                                 | 543 ms: 1.02x faster                                             |
| sqlglot_parse              | 1.24 ms                                                                | 1.22 ms: 1.02x faster                                            |
| scimark_fft                | 355 ms                                                                 | 350 ms: 1.01x faster                                             |
| xml_etree_generate         | 85.3 ms                                                                | 84.1 ms: 1.01x faster                                            |
| deepcopy_reduce            | 3.01 us                                                                | 2.97 us: 1.01x faster                                            |
| 2to3                       | 261 ms                                                                 | 258 ms: 1.01x faster                                             |
| xml_etree_iterparse        | 104 ms                                                                 | 103 ms: 1.01x faster                                             |
| json                       | 5.03 ms                                                                | 4.98 ms: 1.01x faster                                            |
| typing_runtime_protocols   | 108 us                                                                 | 107 us: 1.01x faster                                             |
| unpickle_list              | 4.97 us                                                                | 4.92 us: 1.01x faster                                            |
| logging_silent             | 97.8 ns                                                                | 96.9 ns: 1.01x faster                                            |
| chameleon                  | 6.77 ms                                                                | 6.72 ms: 1.01x faster                                            |
| sympy_expand               | 452 ms                                                                 | 448 ms: 1.01x faster                                             |
| sympy_integrate            | 19.3 ms                                                                | 19.2 ms: 1.01x faster                                            |
| richards                   | 47.0 ms                                                                | 46.9 ms: 1.00x faster                                            |
| python_startup             | 10.0 ms                                                                | 10.1 ms: 1.00x slower                                            |
| regex_dna                  | 217 ms                                                                 | 218 ms: 1.00x slower                                             |
| chaos                      | 58.1 ms                                                                | 58.3 ms: 1.00x slower                                            |
| comprehensions             | 16.0 us                                                                | 16.1 us: 1.00x slower                                            |
| pickle_dict                | 34.9 us                                                                | 35.0 us: 1.00x slower                                            |
| raytrace                   | 258 ms                                                                 | 259 ms: 1.00x slower                                             |
| python_startup_no_site     | 8.67 ms                                                                | 8.70 ms: 1.00x slower                                            |
| async_generators           | 439 ms                                                                 | 442 ms: 1.01x slower                                             |
| go                         | 136 ms                                                                 | 137 ms: 1.01x slower                                             |
| nqueens                    | 77.9 ms                                                                | 78.5 ms: 1.01x slower                                            |
| xml_etree_process          | 58.0 ms                                                                | 58.5 ms: 1.01x slower                                            |
| float                      | 79.3 ms                                                                | 80.0 ms: 1.01x slower                                            |
| unpickle_pure_python       | 211 us                                                                 | 213 us: 1.01x slower                                             |
| scimark_lu                 | 112 ms                                                                 | 113 ms: 1.01x slower                                             |
| deltablue                  | 3.13 ms                                                                | 3.17 ms: 1.01x slower                                            |
| dask                       | 361 ms                                                                 | 366 ms: 1.01x slower                                             |
| asyncio_tcp_ssl            | 1.79 sec                                                               | 1.82 sec: 1.02x slower                                           |
| hexiom                     | 5.97 ms                                                                | 6.09 ms: 1.02x slower                                            |
| nbody                      | 88.2 ms                                                                | 90.1 ms: 1.02x slower                                            |
| docutils                   | 2.60 sec                                                               | 2.66 sec: 1.02x slower                                           |
| asyncio_tcp                | 487 ms                                                                 | 498 ms: 1.02x slower                                             |
| fannkuch                   | 378 ms                                                                 | 388 ms: 1.03x slower                                             |
| mdp                        | 2.52 sec                                                               | 2.59 sec: 1.03x slower                                           |
| meteor_contest             | 106 ms                                                                 | 109 ms: 1.03x slower                                             |
| scimark_sparse_mat_mult    | 4.62 ms                                                                | 4.86 ms: 1.05x slower                                            |
| create_gc_cycles           | 1.46 ms                                                                | 1.54 ms: 1.06x slower                                            |
| async_tree_cpu_io_mixed_tg | 717 ms                                                                 | 771 ms: 1.07x slower                                             |
| gc_traversal               | 3.46 ms                                                                | 3.75 ms: 1.08x slower                                            |
| async_tree_cpu_io_mixed    | 705 ms                                                                 | 763 ms: 1.08x slower                                             |
| async_tree_none_tg         | 441 ms                                                                 | 481 ms: 1.09x slower                                             |
| async_tree_none            | 432 ms                                                                 | 473 ms: 1.10x slower                                             |
| async_tree_memoization_tg  | 569 ms                                                                 | 628 ms: 1.10x slower                                             |
| async_tree_memoization     | 558 ms                                                                 | 628 ms: 1.13x slower                                             |
| async_tree_io_tg           | 1.18 sec                                                               | 1.34 sec: 1.14x slower                                           |
| async_tree_io              | 1.18 sec                                                               | 1.34 sec: 1.14x slower                                           |
| bench_thread_pool          | 817 us                                                                 | 1.20 ms: 1.47x slower                                            |
| Geometric mean             | (ref)                                                                  | 1.00x slower                                                     |

Benchmark hidden because not significant (12): unpickle, json_loads, scimark_sor, logging_format, scimark_monte_carlo, bench_mp_pool, tomli_loads, pickle_pure_python, logging_simple, crypto_pyaes, richards_super, mypy2


# HPT report

- Reliability score: 59.02% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.08x