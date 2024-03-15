
# Results vs. 3.12.0

- fork: faster-cpython
- ref: split_on_oparg_1
- machine: linux-x86_64
- commit hash: 472a3d6
- commit date: 2024-02-15
- overall geometric mean: 1.02x faster \*
- HPT reliability: 99.50%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 277 ms: 1.01x slower                                                         |
| chameleon      | 7.41 ms                                                | 6.84 ms: 1.08x faster                                                        |
| docutils       | 2.77 sec                                               | 2.64 sec: 1.05x faster                                                       |
| tornado_http   | 103 ms                                                 | 96.7 ms: 1.06x faster                                                        |
| Geometric mean | (ref)                                                  | 1.04x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 439 ms: 1.07x faster                                                         |
| async_tree_memoization     | 578 ms                                                 | 559 ms: 1.03x faster                                                         |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 706 ms: 1.03x faster                                                         |
| async_tree_none_tg         | 450 ms                                                 | 444 ms: 1.01x faster                                                         |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 717 ms: 1.01x faster                                                         |
| async_tree_io_tg           | 1.18 sec                                               | 1.18 sec: 1.00x faster                                                       |
| async_tree_io              | 1.16 sec                                               | 1.16 sec: 1.00x slower                                                       |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                                 |

Benchmark hidden because not significant (1): async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 83.0 ms: 1.02x faster                                                        |
| nbody          | 97.0 ms                                                | 101 ms: 1.05x slower                                                         |
| Geometric mean | (ref)                                                  | 1.01x slower                                                                 |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 138 ms: 1.07x faster                                                         |
| regex_effbot   | 3.61 ms                                                | 3.62 ms: 1.00x slower                                                        |
| regex_dna      | 212 ms                                                 | 219 ms: 1.03x slower                                                         |
| regex_v8       | 23.1 ms                                                | 24.6 ms: 1.06x slower                                                        |
| Geometric mean | (ref)                                                  | 1.01x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 299 us: 1.08x faster                                                         |
| tomli_loads          | 2.33 sec                                               | 2.18 sec: 1.07x faster                                                       |
| pickle_dict          | 35.5 us                                                | 33.4 us: 1.06x faster                                                        |
| xml_etree_process    | 61.7 ms                                                | 58.1 ms: 1.06x faster                                                        |
| unpickle             | 15.9 us                                                | 15.1 us: 1.05x faster                                                        |
| xml_etree_generate   | 89.2 ms                                                | 85.2 ms: 1.05x faster                                                        |
| pickle_list          | 5.08 us                                                | 4.91 us: 1.04x faster                                                        |
| json_loads           | 28.5 us                                                | 27.6 us: 1.03x faster                                                        |
| unpickle_list        | 5.29 us                                                | 5.16 us: 1.02x faster                                                        |
| pickle               | 11.6 us                                                | 11.3 us: 1.02x faster                                                        |
| unpickle_pure_python | 230 us                                                 | 225 us: 1.02x faster                                                         |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                                         |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                        |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                                 |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                        |
| python_startup_no_site | 6.94 ms                                                | 8.84 ms: 1.27x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 12.1 ms: 1.02x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 110 us: 1.43x faster                                                         |
| comprehensions             | 21.8 us                                                | 18.0 us: 1.21x faster                                                        |
| logging_simple             | 6.46 us                                                | 5.71 us: 1.13x faster                                                        |
| logging_format             | 7.23 us                                                | 6.39 us: 1.13x faster                                                        |
| deltablue                  | 3.72 ms                                                | 3.31 ms: 1.12x faster                                                        |
| raytrace                   | 312 ms                                                 | 280 ms: 1.11x faster                                                         |
| gc_traversal               | 3.79 ms                                                | 3.47 ms: 1.09x faster                                                        |
| deepcopy_reduce            | 3.35 us                                                | 3.07 us: 1.09x faster                                                        |
| pickle_pure_python         | 324 us                                                 | 299 us: 1.08x faster                                                         |
| chameleon                  | 7.41 ms                                                | 6.84 ms: 1.08x faster                                                        |
| scimark_sor                | 129 ms                                                 | 119 ms: 1.08x faster                                                         |
| regex_compile              | 148 ms                                                 | 138 ms: 1.07x faster                                                         |
| async_tree_none            | 472 ms                                                 | 439 ms: 1.07x faster                                                         |
| sympy_sum                  | 169 ms                                                 | 158 ms: 1.07x faster                                                         |
| sympy_str                  | 300 ms                                                 | 281 ms: 1.07x faster                                                         |
| tomli_loads                | 2.33 sec                                               | 2.18 sec: 1.07x faster                                                       |
| deepcopy                   | 371 us                                                 | 349 us: 1.06x faster                                                         |
| pickle_dict                | 35.5 us                                                | 33.4 us: 1.06x faster                                                        |
| deepcopy_memo              | 40.7 us                                                | 38.3 us: 1.06x faster                                                        |
| xml_etree_process          | 61.7 ms                                                | 58.1 ms: 1.06x faster                                                        |
| tornado_http               | 103 ms                                                 | 96.7 ms: 1.06x faster                                                        |
| pathlib                    | 19.3 ms                                                | 18.3 ms: 1.06x faster                                                        |
| sqlglot_parse              | 1.36 ms                                                | 1.29 ms: 1.06x faster                                                        |
| unpickle                   | 15.9 us                                                | 15.1 us: 1.05x faster                                                        |
| sympy_integrate            | 21.4 ms                                                | 20.4 ms: 1.05x faster                                                        |
| docutils                   | 2.77 sec                                               | 2.64 sec: 1.05x faster                                                       |
| xml_etree_generate         | 89.2 ms                                                | 85.2 ms: 1.05x faster                                                        |
| crypto_pyaes               | 81.9 ms                                                | 78.5 ms: 1.04x faster                                                        |
| generators                 | 31.2 ms                                                | 29.9 ms: 1.04x faster                                                        |
| scimark_fft                | 382 ms                                                 | 367 ms: 1.04x faster                                                         |
| sqlglot_transpile          | 1.68 ms                                                | 1.62 ms: 1.04x faster                                                        |
| json                       | 5.26 ms                                                | 5.06 ms: 1.04x faster                                                        |
| unpack_sequence            | 54.0 ns                                                | 52.0 ns: 1.04x faster                                                        |
| scimark_lu                 | 118 ms                                                 | 114 ms: 1.04x faster                                                         |
| pickle_list                | 5.08 us                                                | 4.91 us: 1.04x faster                                                        |
| async_tree_memoization     | 578 ms                                                 | 559 ms: 1.03x faster                                                         |
| meteor_contest             | 112 ms                                                 | 109 ms: 1.03x faster                                                         |
| json_loads                 | 28.5 us                                                | 27.6 us: 1.03x faster                                                        |
| logging_silent             | 104 ns                                                 | 101 ns: 1.03x faster                                                         |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 706 ms: 1.03x faster                                                         |
| unpickle_list              | 5.29 us                                                | 5.16 us: 1.02x faster                                                        |
| pickle                     | 11.6 us                                                | 11.3 us: 1.02x faster                                                        |
| unpickle_pure_python       | 230 us                                                 | 225 us: 1.02x faster                                                         |
| scimark_monte_carlo        | 75.1 ms                                                | 73.5 ms: 1.02x faster                                                        |
| float                      | 84.7 ms                                                | 83.0 ms: 1.02x faster                                                        |
| xml_etree_parse            | 159 ms                                                 | 156 ms: 1.02x faster                                                         |
| coroutines                 | 23.2 ms                                                | 22.8 ms: 1.02x faster                                                        |
| dask                       | 372 ms                                                 | 365 ms: 1.02x faster                                                         |
| sqlglot_normalize          | 110 ms                                                 | 109 ms: 1.02x faster                                                         |
| mdp                        | 2.63 sec                                               | 2.59 sec: 1.02x faster                                                       |
| async_tree_none_tg         | 450 ms                                                 | 444 ms: 1.01x faster                                                         |
| richards                   | 45.8 ms                                                | 45.2 ms: 1.01x faster                                                        |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 717 ms: 1.01x faster                                                         |
| dulwich_log                | 68.5 ms                                                | 67.7 ms: 1.01x faster                                                        |
| create_gc_cycles           | 1.48 ms                                                | 1.46 ms: 1.01x faster                                                        |
| async_generators           | 463 ms                                                 | 458 ms: 1.01x faster                                                         |
| asyncio_tcp                | 491 ms                                                 | 487 ms: 1.01x faster                                                         |
| async_tree_io_tg           | 1.18 sec                                               | 1.18 sec: 1.00x faster                                                       |
| bench_thread_pool          | 842 us                                                 | 840 us: 1.00x faster                                                         |
| regex_effbot               | 3.61 ms                                                | 3.62 ms: 1.00x slower                                                        |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.79 sec: 1.00x slower                                                       |
| async_tree_io              | 1.16 sec                                               | 1.16 sec: 1.00x slower                                                       |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                        |
| sqlglot_optimize           | 54.8 ms                                                | 55.3 ms: 1.01x slower                                                        |
| 2to3                       | 274 ms                                                 | 277 ms: 1.01x slower                                                         |
| pprint_safe_repr           | 776 ms                                                 | 785 ms: 1.01x slower                                                         |
| mako                       | 11.9 ms                                                | 12.1 ms: 1.02x slower                                                        |
| pyflate                    | 482 ms                                                 | 497 ms: 1.03x slower                                                         |
| regex_dna                  | 212 ms                                                 | 219 ms: 1.03x slower                                                         |
| pprint_pformat             | 1.57 sec                                               | 1.63 sec: 1.04x slower                                                       |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.27 ms: 1.04x slower                                                        |
| nbody                      | 97.0 ms                                                | 101 ms: 1.05x slower                                                         |
| chaos                      | 67.0 ms                                                | 70.6 ms: 1.05x slower                                                        |
| go                         | 139 ms                                                 | 148 ms: 1.06x slower                                                         |
| regex_v8                   | 23.1 ms                                                | 24.6 ms: 1.06x slower                                                        |
| python_startup             | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                        |
| nqueens                    | 83.3 ms                                                | 89.1 ms: 1.07x slower                                                        |
| spectral_norm              | 115 ms                                                 | 126 ms: 1.10x slower                                                         |
| hexiom                     | 6.41 ms                                                | 7.61 ms: 1.19x slower                                                        |
| telco                      | 7.10 ms                                                | 8.61 ms: 1.21x slower                                                        |
| python_startup_no_site     | 6.94 ms                                                | 8.84 ms: 1.27x slower                                                        |
| coverage                   | 72.7 ms                                                | 95.4 ms: 1.31x slower                                                        |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                                 |

Benchmark hidden because not significant (11): async_tree_memoization_tg, xml_etree_iterparse, richards_super, bench_mp_pool, fannkuch, pidigits, sqlite_synth, sympy_expand, asyncio_websockets, pycparser, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.50% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.96x