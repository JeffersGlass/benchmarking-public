# Results vs. base

- fork: faster-cpython
- ref: incremental_gc
- machine: linux-x86_64
- commit hash: 14e3135
- commit date: 2024-01-07
- overall geometric mean: 1.01x faster
- HPT reliability: 98.41%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.05x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 263 ms                                                                 | 270 ms: 1.03x slower                                                       |
| chameleon      | 6.94 ms                                                                | 6.97 ms: 1.00x slower                                                      |
| docutils       | 2.58 sec                                                               | 2.53 sec: 1.02x faster                                                     |
| tornado_http   | 94.2 ms                                                                | 93.6 ms: 1.01x faster                                                      |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.19 sec                                                               | 751 ms: 1.59x faster                                                       |
| async_tree_io              | 1.18 sec                                                               | 804 ms: 1.46x faster                                                       |
| async_tree_none_tg         | 439 ms                                                                 | 347 ms: 1.27x faster                                                       |
| async_tree_memoization_tg  | 572 ms                                                                 | 456 ms: 1.25x faster                                                       |
| async_tree_memoization     | 557 ms                                                                 | 459 ms: 1.21x faster                                                       |
| async_tree_none            | 431 ms                                                                 | 356 ms: 1.21x faster                                                       |
| async_tree_cpu_io_mixed_tg | 716 ms                                                                 | 604 ms: 1.19x faster                                                       |
| async_tree_cpu_io_mixed    | 703 ms                                                                 | 625 ms: 1.12x faster                                                       |
| Geometric mean             | (ref)                                                                  | 1.28x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 86.9 ms                                                                | 91.6 ms: 1.05x slower                                                      |
| float          | 80.0 ms                                                                | 85.8 ms: 1.07x slower                                                      |
| Geometric mean | (ref)                                                                  | 1.04x slower                                                               |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 130 ms                                                                 | 131 ms: 1.01x slower                                                       |
| regex_effbot   | 3.62 ms                                                                | 3.67 ms: 1.01x slower                                                      |
| regex_v8       | 24.9 ms                                                                | 25.5 ms: 1.03x slower                                                      |
| regex_dna      | 218 ms                                                                 | 227 ms: 1.04x slower                                                       |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| unpickle             | 15.5 us                                                                | 14.9 us: 1.04x faster                                                      |
| pickle_list          | 5.09 us                                                                | 5.00 us: 1.02x faster                                                      |
| pickle_dict          | 34.9 us                                                                | 34.6 us: 1.01x faster                                                      |
| unpickle_list        | 5.45 us                                                                | 5.47 us: 1.01x slower                                                      |
| pickle               | 11.5 us                                                                | 11.5 us: 1.01x slower                                                      |
| unpickle_pure_python | 214 us                                                                 | 216 us: 1.01x slower                                                       |
| tomli_loads          | 2.12 sec                                                               | 2.17 sec: 1.02x slower                                                     |
| xml_etree_process    | 59.2 ms                                                                | 60.7 ms: 1.03x slower                                                      |
| xml_etree_generate   | 85.6 ms                                                                | 90.2 ms: 1.05x slower                                                      |
| xml_etree_iterparse  | 105 ms                                                                 | 130 ms: 1.24x slower                                                       |
| xml_etree_parse      | 157 ms                                                                 | 205 ms: 1.30x slower                                                       |
| Geometric mean       | (ref)                                                                  | 1.04x slower                                                               |

Benchmark hidden because not significant (3): pickle_pure_python, json_loads, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 8.68 ms                                                                | 8.55 ms: 1.01x faster                                                      |
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                      |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                                | 11.4 ms: 1.04x slower                                                      |

All benchmarks:
===============

| Benchmark                  | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.19 sec                                                               | 751 ms: 1.59x faster                                                       |
| async_tree_io              | 1.18 sec                                                               | 804 ms: 1.46x faster                                                       |
| async_tree_none_tg         | 439 ms                                                                 | 347 ms: 1.27x faster                                                       |
| async_tree_memoization_tg  | 572 ms                                                                 | 456 ms: 1.25x faster                                                       |
| async_tree_memoization     | 557 ms                                                                 | 459 ms: 1.21x faster                                                       |
| async_tree_none            | 431 ms                                                                 | 356 ms: 1.21x faster                                                       |
| async_tree_cpu_io_mixed_tg | 716 ms                                                                 | 604 ms: 1.19x faster                                                       |
| async_tree_cpu_io_mixed    | 703 ms                                                                 | 625 ms: 1.12x faster                                                       |
| mypy2                      | 837 ms                                                                 | 745 ms: 1.12x faster                                                       |
| unpack_sequence            | 46.5 ns                                                                | 41.8 ns: 1.11x faster                                                      |
| scimark_sor                | 128 ms                                                                 | 119 ms: 1.07x faster                                                       |
| unpickle                   | 15.5 us                                                                | 14.9 us: 1.04x faster                                                      |
| pycparser                  | 1.20 sec                                                               | 1.15 sec: 1.04x faster                                                     |
| nqueens                    | 83.1 ms                                                                | 80.7 ms: 1.03x faster                                                      |
| docutils                   | 2.58 sec                                                               | 2.53 sec: 1.02x faster                                                     |
| coverage                   | 96.4 ms                                                                | 94.6 ms: 1.02x faster                                                      |
| create_gc_cycles           | 1.47 ms                                                                | 1.44 ms: 1.02x faster                                                      |
| pickle_list                | 5.09 us                                                                | 5.00 us: 1.02x faster                                                      |
| scimark_lu                 | 114 ms                                                                 | 112 ms: 1.02x faster                                                       |
| python_startup_no_site     | 8.68 ms                                                                | 8.55 ms: 1.01x faster                                                      |
| dask                       | 360 ms                                                                 | 355 ms: 1.01x faster                                                       |
| pickle_dict                | 34.9 us                                                                | 34.6 us: 1.01x faster                                                      |
| tornado_http               | 94.2 ms                                                                | 93.6 ms: 1.01x faster                                                      |
| asyncio_tcp_ssl            | 1.78 sec                                                               | 1.78 sec: 1.00x faster                                                     |
| sqlglot_normalize          | 107 ms                                                                 | 106 ms: 1.00x faster                                                       |
| asyncio_websockets         | 551 ms                                                                 | 553 ms: 1.00x slower                                                       |
| chameleon                  | 6.94 ms                                                                | 6.97 ms: 1.00x slower                                                      |
| sympy_sum                  | 147 ms                                                                 | 147 ms: 1.00x slower                                                       |
| unpickle_list              | 5.45 us                                                                | 5.47 us: 1.01x slower                                                      |
| pickle                     | 11.5 us                                                                | 11.5 us: 1.01x slower                                                      |
| deltablue                  | 3.20 ms                                                                | 3.22 ms: 1.01x slower                                                      |
| scimark_monte_carlo        | 67.9 ms                                                                | 68.3 ms: 1.01x slower                                                      |
| go                         | 139 ms                                                                 | 140 ms: 1.01x slower                                                       |
| unpickle_pure_python       | 214 us                                                                 | 216 us: 1.01x slower                                                       |
| bench_thread_pool          | 826 us                                                                 | 831 us: 1.01x slower                                                       |
| raytrace                   | 261 ms                                                                 | 263 ms: 1.01x slower                                                       |
| typing_runtime_protocols   | 111 us                                                                 | 112 us: 1.01x slower                                                       |
| dulwich_log                | 65.8 ms                                                                | 66.3 ms: 1.01x slower                                                      |
| meteor_contest             | 107 ms                                                                 | 108 ms: 1.01x slower                                                       |
| regex_compile              | 130 ms                                                                 | 131 ms: 1.01x slower                                                       |
| scimark_fft                | 361 ms                                                                 | 364 ms: 1.01x slower                                                       |
| logging_simple             | 5.63 us                                                                | 5.69 us: 1.01x slower                                                      |
| python_startup             | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                      |
| generators                 | 29.4 ms                                                                | 29.7 ms: 1.01x slower                                                      |
| sympy_integrate            | 19.3 ms                                                                | 19.5 ms: 1.01x slower                                                      |
| regex_effbot               | 3.62 ms                                                                | 3.67 ms: 1.01x slower                                                      |
| pathlib                    | 18.1 ms                                                                | 18.4 ms: 1.01x slower                                                      |
| deepcopy_memo              | 37.9 us                                                                | 38.3 us: 1.01x slower                                                      |
| richards                   | 46.9 ms                                                                | 47.6 ms: 1.02x slower                                                      |
| logging_format             | 6.19 us                                                                | 6.30 us: 1.02x slower                                                      |
| sqlglot_transpile          | 1.56 ms                                                                | 1.59 ms: 1.02x slower                                                      |
| chaos                      | 59.0 ms                                                                | 60.1 ms: 1.02x slower                                                      |
| crypto_pyaes               | 70.7 ms                                                                | 72.0 ms: 1.02x slower                                                      |
| deepcopy_reduce            | 3.07 us                                                                | 3.13 us: 1.02x slower                                                      |
| tomli_loads                | 2.12 sec                                                               | 2.17 sec: 1.02x slower                                                     |
| hexiom                     | 6.07 ms                                                                | 6.20 ms: 1.02x slower                                                      |
| regex_v8                   | 24.9 ms                                                                | 25.5 ms: 1.03x slower                                                      |
| xml_etree_process          | 59.2 ms                                                                | 60.7 ms: 1.03x slower                                                      |
| sqlglot_parse              | 1.24 ms                                                                | 1.27 ms: 1.03x slower                                                      |
| scimark_sparse_mat_mult    | 4.85 ms                                                                | 4.98 ms: 1.03x slower                                                      |
| 2to3                       | 263 ms                                                                 | 270 ms: 1.03x slower                                                       |
| fannkuch                   | 400 ms                                                                 | 415 ms: 1.04x slower                                                       |
| regex_dna                  | 218 ms                                                                 | 227 ms: 1.04x slower                                                       |
| mako                       | 11.0 ms                                                                | 11.4 ms: 1.04x slower                                                      |
| coroutines                 | 22.0 ms                                                                | 22.9 ms: 1.04x slower                                                      |
| telco                      | 8.26 ms                                                                | 8.66 ms: 1.05x slower                                                      |
| xml_etree_generate         | 85.6 ms                                                                | 90.2 ms: 1.05x slower                                                      |
| nbody                      | 86.9 ms                                                                | 91.6 ms: 1.05x slower                                                      |
| mdp                        | 2.55 sec                                                               | 2.72 sec: 1.07x slower                                                     |
| float                      | 80.0 ms                                                                | 85.8 ms: 1.07x slower                                                      |
| gc_traversal               | 3.53 ms                                                                | 3.93 ms: 1.11x slower                                                      |
| xml_etree_iterparse        | 105 ms                                                                 | 130 ms: 1.24x slower                                                       |
| xml_etree_parse            | 157 ms                                                                 | 205 ms: 1.30x slower                                                       |
| Geometric mean             | (ref)                                                                  | 1.01x faster                                                               |

Benchmark hidden because not significant (20): pickle_pure_python, sympy_expand, async_generators, deepcopy, sqlglot_optimize, pprint_safe_repr, json, asyncio_tcp, sympy_str, pidigits, pyflate, json_loads, comprehensions, json_dumps, bench_mp_pool, spectral_norm, pprint_pformat, logging_silent, sqlite_synth, richards_super


# HPT report

- Reliability score: 98.41% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.05x