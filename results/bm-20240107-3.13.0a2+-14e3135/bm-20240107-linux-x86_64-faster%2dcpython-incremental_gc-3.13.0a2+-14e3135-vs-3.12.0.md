
# Results vs. 3.12.0

- fork: faster-cpython
- ref: incremental_gc
- machine: linux-x86_64
- commit hash: 14e3135
- commit date: 2024-01-07
- overall geometric mean: 1.05x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 270 ms: 1.01x faster                                                       |
| chameleon      | 7.41 ms                                                | 6.97 ms: 1.06x faster                                                      |
| docutils       | 2.77 sec                                               | 2.53 sec: 1.10x faster                                                     |
| tornado_http   | 103 ms                                                 | 93.6 ms: 1.10x faster                                                      |
| Geometric mean | (ref)                                                  | 1.07x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.18 sec                                               | 751 ms: 1.58x faster                                                       |
| async_tree_io              | 1.16 sec                                               | 804 ms: 1.44x faster                                                       |
| async_tree_none            | 472 ms                                                 | 356 ms: 1.33x faster                                                       |
| async_tree_none_tg         | 450 ms                                                 | 347 ms: 1.30x faster                                                       |
| async_tree_memoization     | 578 ms                                                 | 459 ms: 1.26x faster                                                       |
| async_tree_memoization_tg  | 575 ms                                                 | 456 ms: 1.26x faster                                                       |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 604 ms: 1.20x faster                                                       |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 625 ms: 1.16x faster                                                       |
| Geometric mean             | (ref)                                                  | 1.31x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 91.6 ms: 1.06x faster                                                      |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x slower                                                       |
| float          | 84.7 ms                                                | 85.8 ms: 1.01x slower                                                      |
| Geometric mean | (ref)                                                  | 1.01x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 131 ms: 1.13x faster                                                       |
| regex_effbot   | 3.61 ms                                                | 3.67 ms: 1.02x slower                                                      |
| regex_dna      | 212 ms                                                 | 227 ms: 1.07x slower                                                       |
| regex_v8       | 23.1 ms                                                | 25.5 ms: 1.10x slower                                                      |
| Geometric mean | (ref)                                                  | 1.01x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 298 us: 1.09x faster                                                       |
| tomli_loads          | 2.33 sec                                               | 2.17 sec: 1.08x faster                                                     |
| unpickle_pure_python | 230 us                                                 | 216 us: 1.07x faster                                                       |
| unpickle             | 15.9 us                                                | 14.9 us: 1.07x faster                                                      |
| pickle_dict          | 35.5 us                                                | 34.6 us: 1.03x faster                                                      |
| pickle_list          | 5.08 us                                                | 5.00 us: 1.02x faster                                                      |
| xml_etree_process    | 61.7 ms                                                | 60.7 ms: 1.02x faster                                                      |
| pickle               | 11.6 us                                                | 11.5 us: 1.01x faster                                                      |
| xml_etree_generate   | 89.2 ms                                                | 90.2 ms: 1.01x slower                                                      |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                      |
| unpickle_list        | 5.29 us                                                | 5.47 us: 1.04x slower                                                      |
| xml_etree_iterparse  | 107 ms                                                 | 130 ms: 1.22x slower                                                       |
| xml_etree_parse      | 159 ms                                                 | 205 ms: 1.28x slower                                                       |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                               |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.06x slower                                                      |
| python_startup_no_site | 6.94 ms                                                | 8.55 ms: 1.23x slower                                                      |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.4 ms: 1.04x faster                                                      |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.18 sec                                               | 751 ms: 1.58x faster                                                       |
| async_tree_io              | 1.16 sec                                               | 804 ms: 1.44x faster                                                       |
| typing_runtime_protocols   | 158 us                                                 | 112 us: 1.41x faster                                                       |
| comprehensions             | 21.8 us                                                | 16.3 us: 1.34x faster                                                      |
| async_tree_none            | 472 ms                                                 | 356 ms: 1.33x faster                                                       |
| async_tree_none_tg         | 450 ms                                                 | 347 ms: 1.30x faster                                                       |
| unpack_sequence            | 54.0 ns                                                | 41.8 ns: 1.29x faster                                                      |
| async_tree_memoization     | 578 ms                                                 | 459 ms: 1.26x faster                                                       |
| async_tree_memoization_tg  | 575 ms                                                 | 456 ms: 1.26x faster                                                       |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 604 ms: 1.20x faster                                                       |
| raytrace                   | 312 ms                                                 | 263 ms: 1.19x faster                                                       |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 625 ms: 1.16x faster                                                       |
| deltablue                  | 3.72 ms                                                | 3.22 ms: 1.15x faster                                                      |
| logging_format             | 7.23 us                                                | 6.30 us: 1.15x faster                                                      |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                                       |
| crypto_pyaes               | 81.9 ms                                                | 72.0 ms: 1.14x faster                                                      |
| logging_simple             | 6.46 us                                                | 5.69 us: 1.14x faster                                                      |
| regex_compile              | 148 ms                                                 | 131 ms: 1.13x faster                                                       |
| sympy_str                  | 300 ms                                                 | 267 ms: 1.12x faster                                                       |
| chaos                      | 67.0 ms                                                | 60.1 ms: 1.11x faster                                                      |
| mypy2                      | 830 ms                                                 | 745 ms: 1.11x faster                                                       |
| scimark_monte_carlo        | 75.1 ms                                                | 68.3 ms: 1.10x faster                                                      |
| tornado_http               | 103 ms                                                 | 93.6 ms: 1.10x faster                                                      |
| docutils                   | 2.77 sec                                               | 2.53 sec: 1.10x faster                                                     |
| sympy_integrate            | 21.4 ms                                                | 19.5 ms: 1.10x faster                                                      |
| pickle_pure_python         | 324 us                                                 | 298 us: 1.09x faster                                                       |
| scimark_sor                | 129 ms                                                 | 119 ms: 1.08x faster                                                       |
| tomli_loads                | 2.33 sec                                               | 2.17 sec: 1.08x faster                                                     |
| deepcopy                   | 371 us                                                 | 347 us: 1.07x faster                                                       |
| sqlglot_parse              | 1.36 ms                                                | 1.27 ms: 1.07x faster                                                      |
| deepcopy_reduce            | 3.35 us                                                | 3.13 us: 1.07x faster                                                      |
| unpickle_pure_python       | 230 us                                                 | 216 us: 1.07x faster                                                       |
| pprint_safe_repr           | 776 ms                                                 | 727 ms: 1.07x faster                                                       |
| unpickle                   | 15.9 us                                                | 14.9 us: 1.07x faster                                                      |
| chameleon                  | 7.41 ms                                                | 6.97 ms: 1.06x faster                                                      |
| deepcopy_memo              | 40.7 us                                                | 38.3 us: 1.06x faster                                                      |
| sqlglot_transpile          | 1.68 ms                                                | 1.59 ms: 1.06x faster                                                      |
| nbody                      | 97.0 ms                                                | 91.6 ms: 1.06x faster                                                      |
| sympy_expand               | 478 ms                                                 | 453 ms: 1.06x faster                                                       |
| pathlib                    | 19.3 ms                                                | 18.4 ms: 1.05x faster                                                      |
| scimark_lu                 | 118 ms                                                 | 112 ms: 1.05x faster                                                       |
| pprint_pformat             | 1.57 sec                                               | 1.49 sec: 1.05x faster                                                     |
| generators                 | 31.2 ms                                                | 29.7 ms: 1.05x faster                                                      |
| spectral_norm              | 115 ms                                                 | 109 ms: 1.05x faster                                                       |
| scimark_fft                | 382 ms                                                 | 364 ms: 1.05x faster                                                       |
| async_generators           | 463 ms                                                 | 442 ms: 1.05x faster                                                       |
| dask                       | 372 ms                                                 | 355 ms: 1.05x faster                                                       |
| mako                       | 11.9 ms                                                | 11.4 ms: 1.04x faster                                                      |
| meteor_contest             | 112 ms                                                 | 108 ms: 1.04x faster                                                       |
| sqlglot_normalize          | 110 ms                                                 | 106 ms: 1.04x faster                                                       |
| hexiom                     | 6.41 ms                                                | 6.20 ms: 1.03x faster                                                      |
| asyncio_tcp                | 491 ms                                                 | 475 ms: 1.03x faster                                                       |
| dulwich_log                | 68.5 ms                                                | 66.3 ms: 1.03x faster                                                      |
| nqueens                    | 83.3 ms                                                | 80.7 ms: 1.03x faster                                                      |
| pyflate                    | 482 ms                                                 | 468 ms: 1.03x faster                                                       |
| create_gc_cycles           | 1.48 ms                                                | 1.44 ms: 1.03x faster                                                      |
| pickle_dict                | 35.5 us                                                | 34.6 us: 1.03x faster                                                      |
| sqlglot_optimize           | 54.8 ms                                                | 53.6 ms: 1.02x faster                                                      |
| pycparser                  | 1.18 sec                                               | 1.15 sec: 1.02x faster                                                     |
| pickle_list                | 5.08 us                                                | 5.00 us: 1.02x faster                                                      |
| xml_etree_process          | 61.7 ms                                                | 60.7 ms: 1.02x faster                                                      |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.98 ms: 1.02x faster                                                      |
| 2to3                       | 274 ms                                                 | 270 ms: 1.01x faster                                                       |
| bench_thread_pool          | 842 us                                                 | 831 us: 1.01x faster                                                       |
| coroutines                 | 23.2 ms                                                | 22.9 ms: 1.01x faster                                                      |
| pickle                     | 11.6 us                                                | 11.5 us: 1.01x faster                                                      |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.78 sec: 1.01x faster                                                     |
| fannkuch                   | 417 ms                                                 | 415 ms: 1.01x faster                                                       |
| pidigits                   | 187 ms                                                 | 187 ms: 1.00x slower                                                       |
| go                         | 139 ms                                                 | 140 ms: 1.00x slower                                                       |
| xml_etree_generate         | 89.2 ms                                                | 90.2 ms: 1.01x slower                                                      |
| float                      | 84.7 ms                                                | 85.8 ms: 1.01x slower                                                      |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                      |
| regex_effbot               | 3.61 ms                                                | 3.67 ms: 1.02x slower                                                      |
| mdp                        | 2.63 sec                                               | 2.72 sec: 1.03x slower                                                     |
| unpickle_list              | 5.29 us                                                | 5.47 us: 1.04x slower                                                      |
| gc_traversal               | 3.79 ms                                                | 3.93 ms: 1.04x slower                                                      |
| richards                   | 45.8 ms                                                | 47.6 ms: 1.04x slower                                                      |
| richards_super             | 51.5 ms                                                | 54.0 ms: 1.05x slower                                                      |
| python_startup             | 9.55 ms                                                | 10.2 ms: 1.06x slower                                                      |
| regex_dna                  | 212 ms                                                 | 227 ms: 1.07x slower                                                       |
| regex_v8                   | 23.1 ms                                                | 25.5 ms: 1.10x slower                                                      |
| xml_etree_iterparse        | 107 ms                                                 | 130 ms: 1.22x slower                                                       |
| telco                      | 7.10 ms                                                | 8.66 ms: 1.22x slower                                                      |
| python_startup_no_site     | 6.94 ms                                                | 8.55 ms: 1.23x slower                                                      |
| xml_etree_parse            | 159 ms                                                 | 205 ms: 1.28x slower                                                       |
| coverage                   | 72.7 ms                                                | 94.6 ms: 1.30x slower                                                      |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                               |

Benchmark hidden because not significant (6): json, json_loads, logging_silent, bench_mp_pool, asyncio_websockets, sqlite_synth
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.94x