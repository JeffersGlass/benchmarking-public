
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: b00e021
- commit date: 2024-01-28
- overall geometric mean: 1.00x faster \*
- HPT reliability: 50.99%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 276 ms: 1.00x slower                                           |
| chameleon      | 7.41 ms                                                | 7.07 ms: 1.05x faster                                          |
| docutils       | 2.77 sec                                               | 2.66 sec: 1.04x faster                                         |
| tornado_http   | 103 ms                                                 | 97.5 ms: 1.05x faster                                          |
| Geometric mean | (ref)                                                  | 1.03x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 442 ms: 1.07x faster                                           |
| async_tree_memoization     | 578 ms                                                 | 564 ms: 1.02x faster                                           |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 708 ms: 1.02x faster                                           |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 717 ms: 1.01x faster                                           |
| async_tree_none_tg         | 450 ms                                                 | 448 ms: 1.00x faster                                           |
| async_tree_io_tg           | 1.18 sec                                               | 1.19 sec: 1.01x slower                                         |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                         |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                   |

Benchmark hidden because not significant (1): async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                           |
| float          | 84.7 ms                                                | 86.2 ms: 1.02x slower                                          |
| nbody          | 97.0 ms                                                | 104 ms: 1.07x slower                                           |
| Geometric mean | (ref)                                                  | 1.03x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 140 ms: 1.06x faster                                           |
| regex_effbot   | 3.61 ms                                                | 3.53 ms: 1.02x faster                                          |
| regex_dna      | 212 ms                                                 | 219 ms: 1.03x slower                                           |
| regex_v8       | 23.1 ms                                                | 24.5 ms: 1.06x slower                                          |
| Geometric mean | (ref)                                                  | 1.00x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 292 us: 1.11x faster                                           |
| unpickle             | 15.9 us                                                | 14.9 us: 1.07x faster                                          |
| tomli_loads          | 2.33 sec                                               | 2.21 sec: 1.06x faster                                         |
| xml_etree_process    | 61.7 ms                                                | 59.5 ms: 1.04x faster                                          |
| pickle_dict          | 35.5 us                                                | 34.3 us: 1.04x faster                                          |
| xml_etree_parse      | 159 ms                                                 | 155 ms: 1.03x faster                                           |
| unpickle_list        | 5.29 us                                                | 5.18 us: 1.02x faster                                          |
| xml_etree_generate   | 89.2 ms                                                | 87.4 ms: 1.02x faster                                          |
| pickle               | 11.6 us                                                | 11.5 us: 1.01x faster                                          |
| json_dumps           | 10.4 ms                                                | 10.3 ms: 1.01x faster                                          |
| json_loads           | 28.5 us                                                | 28.3 us: 1.01x faster                                          |
| unpickle_pure_python | 230 us                                                 | 229 us: 1.00x faster                                           |
| pickle_list          | 5.08 us                                                | 5.14 us: 1.01x slower                                          |
| xml_etree_iterparse  | 107 ms                                                 | 108 ms: 1.02x slower                                           |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                          |
| python_startup_no_site | 6.94 ms                                                | 8.84 ms: 1.27x slower                                          |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 12.7 ms: 1.07x slower                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 111 us: 1.42x faster                                           |
| unpack_sequence            | 54.0 ns                                                | 42.1 ns: 1.28x faster                                          |
| logging_format             | 7.23 us                                                | 6.44 us: 1.12x faster                                          |
| comprehensions             | 21.8 us                                                | 19.4 us: 1.12x faster                                          |
| logging_simple             | 6.46 us                                                | 5.77 us: 1.12x faster                                          |
| pickle_pure_python         | 324 us                                                 | 292 us: 1.11x faster                                           |
| raytrace                   | 312 ms                                                 | 282 ms: 1.11x faster                                           |
| deepcopy_reduce            | 3.35 us                                                | 3.03 us: 1.10x faster                                          |
| deepcopy_memo              | 40.7 us                                                | 37.6 us: 1.08x faster                                          |
| deepcopy                   | 371 us                                                 | 344 us: 1.08x faster                                           |
| unpickle                   | 15.9 us                                                | 14.9 us: 1.07x faster                                          |
| async_tree_none            | 472 ms                                                 | 442 ms: 1.07x faster                                           |
| regex_compile              | 148 ms                                                 | 140 ms: 1.06x faster                                           |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.06x faster                                           |
| pathlib                    | 19.3 ms                                                | 18.3 ms: 1.06x faster                                          |
| sqlglot_parse              | 1.36 ms                                                | 1.29 ms: 1.06x faster                                          |
| tomli_loads                | 2.33 sec                                               | 2.21 sec: 1.06x faster                                         |
| crypto_pyaes               | 81.9 ms                                                | 77.5 ms: 1.06x faster                                          |
| coroutines                 | 23.2 ms                                                | 22.0 ms: 1.06x faster                                          |
| sympy_str                  | 300 ms                                                 | 284 ms: 1.06x faster                                           |
| tornado_http               | 103 ms                                                 | 97.5 ms: 1.05x faster                                          |
| generators                 | 31.2 ms                                                | 29.7 ms: 1.05x faster                                          |
| chameleon                  | 7.41 ms                                                | 7.07 ms: 1.05x faster                                          |
| scimark_sor                | 129 ms                                                 | 123 ms: 1.05x faster                                           |
| sqlglot_transpile          | 1.68 ms                                                | 1.61 ms: 1.04x faster                                          |
| docutils                   | 2.77 sec                                               | 2.66 sec: 1.04x faster                                         |
| xml_etree_process          | 61.7 ms                                                | 59.5 ms: 1.04x faster                                          |
| pickle_dict                | 35.5 us                                                | 34.3 us: 1.04x faster                                          |
| xml_etree_parse            | 159 ms                                                 | 155 ms: 1.03x faster                                           |
| sympy_integrate            | 21.4 ms                                                | 20.9 ms: 1.03x faster                                          |
| async_tree_memoization     | 578 ms                                                 | 564 ms: 1.02x faster                                           |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 708 ms: 1.02x faster                                           |
| scimark_lu                 | 118 ms                                                 | 115 ms: 1.02x faster                                           |
| meteor_contest             | 112 ms                                                 | 110 ms: 1.02x faster                                           |
| gc_traversal               | 3.79 ms                                                | 3.71 ms: 1.02x faster                                          |
| regex_effbot               | 3.61 ms                                                | 3.53 ms: 1.02x faster                                          |
| unpickle_list              | 5.29 us                                                | 5.18 us: 1.02x faster                                          |
| xml_etree_generate         | 89.2 ms                                                | 87.4 ms: 1.02x faster                                          |
| async_generators           | 463 ms                                                 | 454 ms: 1.02x faster                                           |
| logging_silent             | 104 ns                                                 | 102 ns: 1.02x faster                                           |
| dask                       | 372 ms                                                 | 365 ms: 1.02x faster                                           |
| sqlite_synth               | 2.83 us                                                | 2.80 us: 1.01x faster                                          |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 717 ms: 1.01x faster                                           |
| pickle                     | 11.6 us                                                | 11.5 us: 1.01x faster                                          |
| json_dumps                 | 10.4 ms                                                | 10.3 ms: 1.01x faster                                          |
| json_loads                 | 28.5 us                                                | 28.3 us: 1.01x faster                                          |
| unpickle_pure_python       | 230 us                                                 | 229 us: 1.00x faster                                           |
| scimark_fft                | 382 ms                                                 | 381 ms: 1.00x faster                                           |
| async_tree_none_tg         | 450 ms                                                 | 448 ms: 1.00x faster                                           |
| bench_thread_pool          | 842 us                                                 | 839 us: 1.00x faster                                           |
| pidigits                   | 187 ms                                                 | 188 ms: 1.00x slower                                           |
| 2to3                       | 274 ms                                                 | 276 ms: 1.00x slower                                           |
| scimark_monte_carlo        | 75.1 ms                                                | 75.6 ms: 1.01x slower                                          |
| async_tree_io_tg           | 1.18 sec                                               | 1.19 sec: 1.01x slower                                         |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.80 sec: 1.01x slower                                         |
| pickle_list                | 5.08 us                                                | 5.14 us: 1.01x slower                                          |
| create_gc_cycles           | 1.48 ms                                                | 1.49 ms: 1.01x slower                                          |
| xml_etree_iterparse        | 107 ms                                                 | 108 ms: 1.02x slower                                           |
| float                      | 84.7 ms                                                | 86.2 ms: 1.02x slower                                          |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                         |
| richards                   | 45.8 ms                                                | 46.8 ms: 1.02x slower                                          |
| sqlglot_optimize           | 54.8 ms                                                | 56.1 ms: 1.02x slower                                          |
| pycparser                  | 1.18 sec                                               | 1.21 sec: 1.03x slower                                         |
| richards_super             | 51.5 ms                                                | 53.0 ms: 1.03x slower                                          |
| pprint_safe_repr           | 776 ms                                                 | 798 ms: 1.03x slower                                           |
| mdp                        | 2.63 sec                                               | 2.71 sec: 1.03x slower                                         |
| regex_dna                  | 212 ms                                                 | 219 ms: 1.03x slower                                           |
| fannkuch                   | 417 ms                                                 | 432 ms: 1.04x slower                                           |
| pprint_pformat             | 1.57 sec                                               | 1.65 sec: 1.05x slower                                         |
| regex_v8                   | 23.1 ms                                                | 24.5 ms: 1.06x slower                                          |
| mako                       | 11.9 ms                                                | 12.7 ms: 1.07x slower                                          |
| nbody                      | 97.0 ms                                                | 104 ms: 1.07x slower                                           |
| python_startup             | 9.55 ms                                                | 10.2 ms: 1.07x slower                                          |
| pyflate                    | 482 ms                                                 | 517 ms: 1.07x slower                                           |
| chaos                      | 67.0 ms                                                | 71.8 ms: 1.07x slower                                          |
| go                         | 139 ms                                                 | 150 ms: 1.07x slower                                           |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.49 ms: 1.09x slower                                          |
| deltablue                  | 3.72 ms                                                | 4.06 ms: 1.09x slower                                          |
| nqueens                    | 83.3 ms                                                | 91.4 ms: 1.10x slower                                          |
| spectral_norm              | 115 ms                                                 | 139 ms: 1.21x slower                                           |
| telco                      | 7.10 ms                                                | 8.65 ms: 1.22x slower                                          |
| hexiom                     | 6.41 ms                                                | 8.05 ms: 1.26x slower                                          |
| python_startup_no_site     | 6.94 ms                                                | 8.84 ms: 1.27x slower                                          |
| coverage                   | 72.7 ms                                                | 93.4 ms: 1.28x slower                                          |
| Geometric mean             | (ref)                                                  | 1.00x faster                                                   |

Benchmark hidden because not significant (9): sqlglot_normalize, dulwich_log, sympy_expand, bench_mp_pool, async_tree_memoization_tg, asyncio_websockets, json, asyncio_tcp, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 50.99% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.97x