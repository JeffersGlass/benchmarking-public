
# Results vs. 3.12.0

- fork: mdboom
- ref: force_mimalloc
- machine: linux-x86_64
- commit hash: f8250a4
- commit date: 2024-02-14
- overall geometric mean: 1.05x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 258 ms: 1.06x faster                                             |
| chameleon      | 7.41 ms                                                | 6.72 ms: 1.10x faster                                            |
| docutils       | 2.77 sec                                               | 2.66 sec: 1.04x faster                                           |
| tornado_http   | 103 ms                                                 | 91.7 ms: 1.12x faster                                            |
| Geometric mean | (ref)                                                  | 1.08x faster                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 726 ms                                                 | 763 ms: 1.05x slower                                             |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 771 ms: 1.06x slower                                             |
| async_tree_none_tg         | 450 ms                                                 | 481 ms: 1.07x slower                                             |
| async_tree_memoization     | 578 ms                                                 | 628 ms: 1.09x slower                                             |
| async_tree_memoization_tg  | 575 ms                                                 | 628 ms: 1.09x slower                                             |
| async_tree_io_tg           | 1.18 sec                                               | 1.34 sec: 1.14x slower                                           |
| async_tree_io              | 1.16 sec                                               | 1.34 sec: 1.16x slower                                           |
| Geometric mean             | (ref)                                                  | 1.08x slower                                                     |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 90.1 ms: 1.08x faster                                            |
| float          | 84.7 ms                                                | 80.0 ms: 1.06x faster                                            |
| pidigits       | 187 ms                                                 | 181 ms: 1.03x faster                                             |
| Geometric mean | (ref)                                                  | 1.06x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 126 ms: 1.18x faster                                             |
| regex_effbot   | 3.61 ms                                                | 3.50 ms: 1.03x faster                                            |
| regex_dna      | 212 ms                                                 | 218 ms: 1.03x slower                                             |
| regex_v8       | 23.1 ms                                                | 24.5 ms: 1.06x slower                                            |
| Geometric mean | (ref)                                                  | 1.03x faster                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.08 sec: 1.12x faster                                           |
| pickle_pure_python   | 324 us                                                 | 292 us: 1.11x faster                                             |
| unpickle_pure_python | 230 us                                                 | 213 us: 1.08x faster                                             |
| unpickle_list        | 5.29 us                                                | 4.92 us: 1.07x faster                                            |
| xml_etree_generate   | 89.2 ms                                                | 84.1 ms: 1.06x faster                                            |
| xml_etree_process    | 61.7 ms                                                | 58.5 ms: 1.06x faster                                            |
| json_loads           | 28.5 us                                                | 27.1 us: 1.05x faster                                            |
| xml_etree_iterparse  | 107 ms                                                 | 103 ms: 1.03x faster                                             |
| xml_etree_parse      | 159 ms                                                 | 155 ms: 1.03x faster                                             |
| json_dumps           | 10.4 ms                                                | 10.2 ms: 1.02x faster                                            |
| pickle_dict          | 35.5 us                                                | 35.0 us: 1.01x faster                                            |
| pickle               | 11.6 us                                                | 11.5 us: 1.01x faster                                            |
| pickle_list          | 5.08 us                                                | 5.11 us: 1.00x slower                                            |
| unpickle             | 15.9 us                                                | 16.1 us: 1.02x slower                                            |
| Geometric mean       | (ref)                                                  | 1.05x faster                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.05x slower                                            |
| python_startup_no_site | 6.94 ms                                                | 8.70 ms: 1.25x slower                                            |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 10.2 ms: 1.17x faster                                            |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 107 us: 1.48x faster                                             |
| comprehensions             | 21.8 us                                                | 16.1 us: 1.35x faster                                            |
| unpack_sequence            | 54.0 ns                                                | 40.8 ns: 1.32x faster                                            |
| raytrace                   | 312 ms                                                 | 259 ms: 1.21x faster                                             |
| regex_compile              | 148 ms                                                 | 126 ms: 1.18x faster                                             |
| logging_format             | 7.23 us                                                | 6.17 us: 1.17x faster                                            |
| mako                       | 11.9 ms                                                | 10.2 ms: 1.17x faster                                            |
| deltablue                  | 3.72 ms                                                | 3.17 ms: 1.17x faster                                            |
| sympy_sum                  | 169 ms                                                 | 145 ms: 1.17x faster                                             |
| crypto_pyaes               | 81.9 ms                                                | 71.1 ms: 1.15x faster                                            |
| sympy_str                  | 300 ms                                                 | 260 ms: 1.15x faster                                             |
| logging_simple             | 6.46 us                                                | 5.62 us: 1.15x faster                                            |
| chaos                      | 67.0 ms                                                | 58.3 ms: 1.15x faster                                            |
| spectral_norm              | 115 ms                                                 | 101 ms: 1.14x faster                                             |
| scimark_monte_carlo        | 75.1 ms                                                | 66.1 ms: 1.14x faster                                            |
| deepcopy_reduce            | 3.35 us                                                | 2.97 us: 1.13x faster                                            |
| tomli_loads                | 2.33 sec                                               | 2.08 sec: 1.12x faster                                           |
| tornado_http               | 103 ms                                                 | 91.7 ms: 1.12x faster                                            |
| pathlib                    | 19.3 ms                                                | 17.3 ms: 1.12x faster                                            |
| sqlglot_parse              | 1.36 ms                                                | 1.22 ms: 1.12x faster                                            |
| deepcopy                   | 371 us                                                 | 332 us: 1.12x faster                                             |
| deepcopy_memo              | 40.7 us                                                | 36.5 us: 1.12x faster                                            |
| sympy_integrate            | 21.4 ms                                                | 19.2 ms: 1.11x faster                                            |
| pickle_pure_python         | 324 us                                                 | 292 us: 1.11x faster                                             |
| sqlglot_transpile          | 1.68 ms                                                | 1.52 ms: 1.10x faster                                            |
| chameleon                  | 7.41 ms                                                | 6.72 ms: 1.10x faster                                            |
| pyflate                    | 482 ms                                                 | 438 ms: 1.10x faster                                             |
| scimark_sor                | 129 ms                                                 | 117 ms: 1.10x faster                                             |
| pprint_safe_repr           | 776 ms                                                 | 710 ms: 1.09x faster                                             |
| scimark_fft                | 382 ms                                                 | 350 ms: 1.09x faster                                             |
| pprint_pformat             | 1.57 sec                                               | 1.44 sec: 1.09x faster                                           |
| sqlglot_normalize          | 110 ms                                                 | 102 ms: 1.08x faster                                             |
| dulwich_log                | 68.5 ms                                                | 63.4 ms: 1.08x faster                                            |
| unpickle_pure_python       | 230 us                                                 | 213 us: 1.08x faster                                             |
| logging_silent             | 104 ns                                                 | 96.9 ns: 1.08x faster                                            |
| generators                 | 31.2 ms                                                | 29.0 ms: 1.08x faster                                            |
| nbody                      | 97.0 ms                                                | 90.1 ms: 1.08x faster                                            |
| coroutines                 | 23.2 ms                                                | 21.5 ms: 1.08x faster                                            |
| unpickle_list              | 5.29 us                                                | 4.92 us: 1.07x faster                                            |
| fannkuch                   | 417 ms                                                 | 388 ms: 1.07x faster                                             |
| sympy_expand               | 478 ms                                                 | 448 ms: 1.07x faster                                             |
| pycparser                  | 1.18 sec                                               | 1.10 sec: 1.07x faster                                           |
| sqlglot_optimize           | 54.8 ms                                                | 51.5 ms: 1.06x faster                                            |
| 2to3                       | 274 ms                                                 | 258 ms: 1.06x faster                                             |
| nqueens                    | 83.3 ms                                                | 78.5 ms: 1.06x faster                                            |
| xml_etree_generate         | 89.2 ms                                                | 84.1 ms: 1.06x faster                                            |
| float                      | 84.7 ms                                                | 80.0 ms: 1.06x faster                                            |
| json                       | 5.26 ms                                                | 4.98 ms: 1.06x faster                                            |
| xml_etree_process          | 61.7 ms                                                | 58.5 ms: 1.06x faster                                            |
| json_loads                 | 28.5 us                                                | 27.1 us: 1.05x faster                                            |
| hexiom                     | 6.41 ms                                                | 6.09 ms: 1.05x faster                                            |
| async_generators           | 463 ms                                                 | 442 ms: 1.05x faster                                             |
| scimark_lu                 | 118 ms                                                 | 113 ms: 1.05x faster                                             |
| docutils                   | 2.77 sec                                               | 2.66 sec: 1.04x faster                                           |
| sqlite_synth               | 2.83 us                                                | 2.72 us: 1.04x faster                                            |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.86 ms: 1.04x faster                                            |
| xml_etree_iterparse        | 107 ms                                                 | 103 ms: 1.03x faster                                             |
| pidigits                   | 187 ms                                                 | 181 ms: 1.03x faster                                             |
| regex_effbot               | 3.61 ms                                                | 3.50 ms: 1.03x faster                                            |
| xml_etree_parse            | 159 ms                                                 | 155 ms: 1.03x faster                                             |
| meteor_contest             | 112 ms                                                 | 109 ms: 1.03x faster                                             |
| json_dumps                 | 10.4 ms                                                | 10.2 ms: 1.02x faster                                            |
| go                         | 139 ms                                                 | 137 ms: 1.02x faster                                             |
| mdp                        | 2.63 sec                                               | 2.59 sec: 1.02x faster                                           |
| dask                       | 372 ms                                                 | 366 ms: 1.02x faster                                             |
| asyncio_websockets         | 551 ms                                                 | 543 ms: 1.02x faster                                             |
| pickle_dict                | 35.5 us                                                | 35.0 us: 1.01x faster                                            |
| gc_traversal               | 3.79 ms                                                | 3.75 ms: 1.01x faster                                            |
| pickle                     | 11.6 us                                                | 11.5 us: 1.01x faster                                            |
| pickle_list                | 5.08 us                                                | 5.11 us: 1.00x slower                                            |
| unpickle                   | 15.9 us                                                | 16.1 us: 1.02x slower                                            |
| asyncio_tcp                | 491 ms                                                 | 498 ms: 1.02x slower                                             |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.82 sec: 1.02x slower                                           |
| richards                   | 45.8 ms                                                | 46.9 ms: 1.02x slower                                            |
| regex_dna                  | 212 ms                                                 | 218 ms: 1.03x slower                                             |
| richards_super             | 51.5 ms                                                | 53.5 ms: 1.04x slower                                            |
| create_gc_cycles           | 1.48 ms                                                | 1.54 ms: 1.05x slower                                            |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 763 ms: 1.05x slower                                             |
| python_startup             | 9.55 ms                                                | 10.1 ms: 1.05x slower                                            |
| regex_v8                   | 23.1 ms                                                | 24.5 ms: 1.06x slower                                            |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 771 ms: 1.06x slower                                             |
| async_tree_none_tg         | 450 ms                                                 | 481 ms: 1.07x slower                                             |
| async_tree_memoization     | 578 ms                                                 | 628 ms: 1.09x slower                                             |
| async_tree_memoization_tg  | 575 ms                                                 | 628 ms: 1.09x slower                                             |
| async_tree_io_tg           | 1.18 sec                                               | 1.34 sec: 1.14x slower                                           |
| telco                      | 7.10 ms                                                | 8.18 ms: 1.15x slower                                            |
| async_tree_io              | 1.16 sec                                               | 1.34 sec: 1.16x slower                                           |
| python_startup_no_site     | 6.94 ms                                                | 8.70 ms: 1.25x slower                                            |
| coverage                   | 72.7 ms                                                | 95.5 ms: 1.31x slower                                            |
| bench_thread_pool          | 842 us                                                 | 1.20 ms: 1.43x slower                                            |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                     |

Benchmark hidden because not significant (3): bench_mp_pool, async_tree_none, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.01x