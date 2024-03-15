# Results vs. base

- fork: faster-cpython
- ref: incremental_gc
- machine: linux-x86_64
- commit hash: 4cde149
- commit date: 2024-01-07
- overall geometric mean: 1.01x faster
- HPT reliability: 94.08%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.04x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 263 ms                                                                 | 270 ms: 1.03x slower                                                       |
| chameleon      | 6.94 ms                                                                | 7.02 ms: 1.01x slower                                                      |
| docutils       | 2.58 sec                                                               | 2.53 sec: 1.02x faster                                                     |
| tornado_http   | 94.2 ms                                                                | 93.6 ms: 1.01x faster                                                      |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.19 sec                                                               | 760 ms: 1.57x faster                                                       |
| async_tree_io              | 1.18 sec                                                               | 806 ms: 1.46x faster                                                       |
| async_tree_none_tg         | 439 ms                                                                 | 349 ms: 1.26x faster                                                       |
| async_tree_memoization_tg  | 572 ms                                                                 | 459 ms: 1.25x faster                                                       |
| async_tree_none            | 431 ms                                                                 | 358 ms: 1.21x faster                                                       |
| async_tree_memoization     | 557 ms                                                                 | 463 ms: 1.21x faster                                                       |
| async_tree_cpu_io_mixed_tg | 716 ms                                                                 | 607 ms: 1.18x faster                                                       |
| async_tree_cpu_io_mixed    | 703 ms                                                                 | 631 ms: 1.11x faster                                                       |
| Geometric mean             | (ref)                                                                  | 1.27x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                                 | 187 ms: 1.00x faster                                                       |
| nbody          | 86.9 ms                                                                | 91.9 ms: 1.06x slower                                                      |
| float          | 80.0 ms                                                                | 86.6 ms: 1.08x slower                                                      |
| Geometric mean | (ref)                                                                  | 1.05x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_dna      | 218 ms                                                                 | 223 ms: 1.02x slower                                                       |
| regex_compile  | 130 ms                                                                 | 133 ms: 1.02x slower                                                       |
| regex_effbot   | 3.62 ms                                                                | 3.78 ms: 1.04x slower                                                      |
| regex_v8       | 24.9 ms                                                                | 26.0 ms: 1.05x slower                                                      |
| Geometric mean | (ref)                                                                  | 1.03x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| unpickle             | 15.5 us                                                                | 15.1 us: 1.02x faster                                                      |
| pickle_list          | 5.09 us                                                                | 4.97 us: 1.02x faster                                                      |
| pickle_dict          | 34.9 us                                                                | 34.5 us: 1.01x faster                                                      |
| json_loads           | 28.4 us                                                                | 28.2 us: 1.01x faster                                                      |
| json_dumps           | 10.5 ms                                                                | 10.6 ms: 1.00x slower                                                      |
| pickle               | 11.5 us                                                                | 11.5 us: 1.01x slower                                                      |
| unpickle_pure_python | 214 us                                                                 | 216 us: 1.01x slower                                                       |
| unpickle_list        | 5.45 us                                                                | 5.49 us: 1.01x slower                                                      |
| tomli_loads          | 2.12 sec                                                               | 2.15 sec: 1.01x slower                                                     |
| xml_etree_process    | 59.2 ms                                                                | 61.1 ms: 1.03x slower                                                      |
| xml_etree_generate   | 85.6 ms                                                                | 90.5 ms: 1.06x slower                                                      |
| xml_etree_iterparse  | 105 ms                                                                 | 132 ms: 1.25x slower                                                       |
| xml_etree_parse      | 157 ms                                                                 | 207 ms: 1.31x slower                                                       |
| Geometric mean       | (ref)                                                                  | 1.04x slower                                                               |

Benchmark hidden because not significant (1): pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 8.68 ms                                                                | 8.56 ms: 1.01x faster                                                      |
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                      |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                                | 11.4 ms: 1.04x slower                                                      |

All benchmarks:
===============

| Benchmark                  | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.19 sec                                                               | 760 ms: 1.57x faster                                                       |
| async_tree_io              | 1.18 sec                                                               | 806 ms: 1.46x faster                                                       |
| async_tree_none_tg         | 439 ms                                                                 | 349 ms: 1.26x faster                                                       |
| async_tree_memoization_tg  | 572 ms                                                                 | 459 ms: 1.25x faster                                                       |
| async_tree_none            | 431 ms                                                                 | 358 ms: 1.21x faster                                                       |
| async_tree_memoization     | 557 ms                                                                 | 463 ms: 1.21x faster                                                       |
| async_tree_cpu_io_mixed_tg | 716 ms                                                                 | 607 ms: 1.18x faster                                                       |
| mypy2                      | 837 ms                                                                 | 748 ms: 1.12x faster                                                       |
| async_tree_cpu_io_mixed    | 703 ms                                                                 | 631 ms: 1.11x faster                                                       |
| scimark_sor                | 128 ms                                                                 | 120 ms: 1.06x faster                                                       |
| nqueens                    | 83.1 ms                                                                | 81.1 ms: 1.02x faster                                                      |
| unpickle                   | 15.5 us                                                                | 15.1 us: 1.02x faster                                                      |
| pickle_list                | 5.09 us                                                                | 4.97 us: 1.02x faster                                                      |
| docutils                   | 2.58 sec                                                               | 2.53 sec: 1.02x faster                                                     |
| create_gc_cycles           | 1.47 ms                                                                | 1.44 ms: 1.02x faster                                                      |
| async_generators           | 443 ms                                                                 | 436 ms: 1.01x faster                                                       |
| python_startup_no_site     | 8.68 ms                                                                | 8.56 ms: 1.01x faster                                                      |
| pickle_dict                | 34.9 us                                                                | 34.5 us: 1.01x faster                                                      |
| json                       | 5.24 ms                                                                | 5.18 ms: 1.01x faster                                                      |
| logging_silent             | 104 ns                                                                 | 103 ns: 1.01x faster                                                       |
| dask                       | 360 ms                                                                 | 356 ms: 1.01x faster                                                       |
| scimark_lu                 | 114 ms                                                                 | 113 ms: 1.01x faster                                                       |
| pycparser                  | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                                     |
| json_loads                 | 28.4 us                                                                | 28.2 us: 1.01x faster                                                      |
| tornado_http               | 94.2 ms                                                                | 93.6 ms: 1.01x faster                                                      |
| go                         | 139 ms                                                                 | 138 ms: 1.01x faster                                                       |
| chaos                      | 59.0 ms                                                                | 58.8 ms: 1.00x faster                                                      |
| pyflate                    | 468 ms                                                                 | 466 ms: 1.00x faster                                                       |
| sqlglot_normalize          | 107 ms                                                                 | 106 ms: 1.00x faster                                                       |
| pidigits                   | 187 ms                                                                 | 187 ms: 1.00x faster                                                       |
| comprehensions             | 16.3 us                                                                | 16.3 us: 1.00x slower                                                      |
| json_dumps                 | 10.5 ms                                                                | 10.6 ms: 1.00x slower                                                      |
| sqlglot_parse              | 1.24 ms                                                                | 1.25 ms: 1.00x slower                                                      |
| deepcopy                   | 348 us                                                                 | 349 us: 1.00x slower                                                       |
| pickle                     | 11.5 us                                                                | 11.5 us: 1.01x slower                                                      |
| generators                 | 29.4 ms                                                                | 29.6 ms: 1.01x slower                                                      |
| scimark_monte_carlo        | 67.9 ms                                                                | 68.4 ms: 1.01x slower                                                      |
| pathlib                    | 18.1 ms                                                                | 18.3 ms: 1.01x slower                                                      |
| unpickle_pure_python       | 214 us                                                                 | 216 us: 1.01x slower                                                       |
| deltablue                  | 3.20 ms                                                                | 3.23 ms: 1.01x slower                                                      |
| unpickle_list              | 5.45 us                                                                | 5.49 us: 1.01x slower                                                      |
| sympy_sum                  | 147 ms                                                                 | 148 ms: 1.01x slower                                                       |
| dulwich_log                | 65.8 ms                                                                | 66.5 ms: 1.01x slower                                                      |
| chameleon                  | 6.94 ms                                                                | 7.02 ms: 1.01x slower                                                      |
| deepcopy_memo              | 37.9 us                                                                | 38.3 us: 1.01x slower                                                      |
| python_startup             | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                      |
| deepcopy_reduce            | 3.07 us                                                                | 3.11 us: 1.01x slower                                                      |
| hexiom                     | 6.07 ms                                                                | 6.15 ms: 1.01x slower                                                      |
| sympy_str                  | 267 ms                                                                 | 270 ms: 1.01x slower                                                       |
| tomli_loads                | 2.12 sec                                                               | 2.15 sec: 1.01x slower                                                     |
| sqlite_synth               | 2.82 us                                                                | 2.86 us: 1.01x slower                                                      |
| logging_simple             | 5.63 us                                                                | 5.71 us: 1.01x slower                                                      |
| bench_thread_pool          | 826 us                                                                 | 837 us: 1.01x slower                                                       |
| sympy_integrate            | 19.3 ms                                                                | 19.6 ms: 1.01x slower                                                      |
| logging_format             | 6.19 us                                                                | 6.29 us: 1.01x slower                                                      |
| asyncio_tcp                | 475 ms                                                                 | 483 ms: 1.02x slower                                                       |
| richards                   | 46.9 ms                                                                | 47.7 ms: 1.02x slower                                                      |
| scimark_sparse_mat_mult    | 4.85 ms                                                                | 4.93 ms: 1.02x slower                                                      |
| regex_dna                  | 218 ms                                                                 | 223 ms: 1.02x slower                                                       |
| telco                      | 8.26 ms                                                                | 8.44 ms: 1.02x slower                                                      |
| meteor_contest             | 107 ms                                                                 | 110 ms: 1.02x slower                                                       |
| crypto_pyaes               | 70.7 ms                                                                | 72.3 ms: 1.02x slower                                                      |
| regex_compile              | 130 ms                                                                 | 133 ms: 1.02x slower                                                       |
| scimark_fft                | 361 ms                                                                 | 370 ms: 1.03x slower                                                       |
| 2to3                       | 263 ms                                                                 | 270 ms: 1.03x slower                                                       |
| xml_etree_process          | 59.2 ms                                                                | 61.1 ms: 1.03x slower                                                      |
| coroutines                 | 22.0 ms                                                                | 22.7 ms: 1.03x slower                                                      |
| typing_runtime_protocols   | 111 us                                                                 | 115 us: 1.03x slower                                                       |
| spectral_norm              | 109 ms                                                                 | 113 ms: 1.04x slower                                                       |
| mako                       | 11.0 ms                                                                | 11.4 ms: 1.04x slower                                                      |
| regex_effbot               | 3.62 ms                                                                | 3.78 ms: 1.04x slower                                                      |
| regex_v8                   | 24.9 ms                                                                | 26.0 ms: 1.05x slower                                                      |
| fannkuch                   | 400 ms                                                                 | 420 ms: 1.05x slower                                                       |
| xml_etree_generate         | 85.6 ms                                                                | 90.5 ms: 1.06x slower                                                      |
| nbody                      | 86.9 ms                                                                | 91.9 ms: 1.06x slower                                                      |
| float                      | 80.0 ms                                                                | 86.6 ms: 1.08x slower                                                      |
| gc_traversal               | 3.53 ms                                                                | 3.82 ms: 1.08x slower                                                      |
| unpack_sequence            | 46.5 ns                                                                | 50.4 ns: 1.08x slower                                                      |
| xml_etree_iterparse        | 105 ms                                                                 | 132 ms: 1.25x slower                                                       |
| xml_etree_parse            | 157 ms                                                                 | 207 ms: 1.31x slower                                                       |
| Geometric mean             | (ref)                                                                  | 1.01x faster                                                               |

Benchmark hidden because not significant (13): coverage, pprint_safe_repr, sqlglot_optimize, sqlglot_transpile, pprint_pformat, bench_mp_pool, asyncio_tcp_ssl, pickle_pure_python, asyncio_websockets, raytrace, mdp, sympy_expand, richards_super


# HPT report

- Reliability score: 94.08% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.04x