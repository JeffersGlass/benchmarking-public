
# Results vs. 3.12.0

- fork: faster-cpython
- ref: better_set_ip_check_
- machine: linux-x86_64
- commit hash: 4d59a84
- commit date: 2024-02-09
- overall geometric mean: 1.02x slower \*
- HPT reliability: 99.99%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 282 ms: 1.03x slower                                                             |
| chameleon      | 7.41 ms                                                | 7.34 ms: 1.01x faster                                                            |
| docutils       | 2.77 sec                                               | 2.70 sec: 1.03x faster                                                           |
| tornado_http   | 103 ms                                                 | 98.5 ms: 1.04x faster                                                            |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 452 ms: 1.04x faster                                                             |
| async_tree_none_tg         | 450 ms                                                 | 454 ms: 1.01x slower                                                             |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 737 ms: 1.02x slower                                                             |
| async_tree_memoization_tg  | 575 ms                                                 | 591 ms: 1.03x slower                                                             |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                           |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.04x slower                                                           |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.01x slower                                                             |
| float          | 84.7 ms                                                | 91.8 ms: 1.08x slower                                                            |
| nbody          | 97.0 ms                                                | 114 ms: 1.17x slower                                                             |
| Geometric mean | (ref)                                                  | 1.09x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.66 ms: 1.01x slower                                                            |
| regex_compile  | 148 ms                                                 | 151 ms: 1.02x slower                                                             |
| regex_dna      | 212 ms                                                 | 227 ms: 1.07x slower                                                             |
| regex_v8       | 23.1 ms                                                | 25.2 ms: 1.09x slower                                                            |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle             | 15.9 us                                                | 14.7 us: 1.08x faster                                                            |
| pickle_pure_python   | 324 us                                                 | 303 us: 1.07x faster                                                             |
| unpickle_list        | 5.29 us                                                | 5.17 us: 1.02x faster                                                            |
| xml_etree_process    | 61.7 ms                                                | 60.5 ms: 1.02x faster                                                            |
| pickle               | 11.6 us                                                | 11.4 us: 1.01x faster                                                            |
| json_loads           | 28.5 us                                                | 28.1 us: 1.01x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                             |
| xml_etree_generate   | 89.2 ms                                                | 88.8 ms: 1.00x faster                                                            |
| pickle_dict          | 35.5 us                                                | 35.8 us: 1.01x slower                                                            |
| unpickle_pure_python | 230 us                                                 | 233 us: 1.01x slower                                                             |
| tomli_loads          | 2.33 sec                                               | 2.37 sec: 1.02x slower                                                           |
| json_dumps           | 10.4 ms                                                | 10.6 ms: 1.03x slower                                                            |
| xml_etree_iterparse  | 107 ms                                                 | 110 ms: 1.03x slower                                                             |
| pickle_list          | 5.08 us                                                | 5.26 us: 1.03x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 8.74 ms: 1.26x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 13.6 ms: 1.14x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 117 us: 1.35x faster                                                             |
| unpack_sequence            | 54.0 ns                                                | 42.7 ns: 1.26x faster                                                            |
| unpickle                   | 15.9 us                                                | 14.7 us: 1.08x faster                                                            |
| logging_simple             | 6.46 us                                                | 6.02 us: 1.07x faster                                                            |
| pickle_pure_python         | 324 us                                                 | 303 us: 1.07x faster                                                             |
| logging_format             | 7.23 us                                                | 6.79 us: 1.07x faster                                                            |
| deepcopy_reduce            | 3.35 us                                                | 3.14 us: 1.06x faster                                                            |
| generators                 | 31.2 ms                                                | 29.4 ms: 1.06x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.06x faster                                                             |
| comprehensions             | 21.8 us                                                | 20.6 us: 1.06x faster                                                            |
| raytrace                   | 312 ms                                                 | 297 ms: 1.05x faster                                                             |
| pathlib                    | 19.3 ms                                                | 18.5 ms: 1.04x faster                                                            |
| async_tree_none            | 472 ms                                                 | 452 ms: 1.04x faster                                                             |
| tornado_http               | 103 ms                                                 | 98.5 ms: 1.04x faster                                                            |
| deepcopy                   | 371 us                                                 | 357 us: 1.04x faster                                                             |
| coroutines                 | 23.2 ms                                                | 22.4 ms: 1.03x faster                                                            |
| async_generators           | 463 ms                                                 | 450 ms: 1.03x faster                                                             |
| sympy_str                  | 300 ms                                                 | 292 ms: 1.03x faster                                                             |
| scimark_sor                | 129 ms                                                 | 126 ms: 1.03x faster                                                             |
| docutils                   | 2.77 sec                                               | 2.70 sec: 1.03x faster                                                           |
| gc_traversal               | 3.79 ms                                                | 3.70 ms: 1.02x faster                                                            |
| sqlglot_parse              | 1.36 ms                                                | 1.33 ms: 1.02x faster                                                            |
| unpickle_list              | 5.29 us                                                | 5.17 us: 1.02x faster                                                            |
| xml_etree_process          | 61.7 ms                                                | 60.5 ms: 1.02x faster                                                            |
| pickle                     | 11.6 us                                                | 11.4 us: 1.01x faster                                                            |
| json_loads                 | 28.5 us                                                | 28.1 us: 1.01x faster                                                            |
| sqlglot_transpile          | 1.68 ms                                                | 1.66 ms: 1.01x faster                                                            |
| xml_etree_parse            | 159 ms                                                 | 158 ms: 1.01x faster                                                             |
| sympy_integrate            | 21.4 ms                                                | 21.2 ms: 1.01x faster                                                            |
| chameleon                  | 7.41 ms                                                | 7.34 ms: 1.01x faster                                                            |
| deepcopy_memo              | 40.7 us                                                | 40.3 us: 1.01x faster                                                            |
| create_gc_cycles           | 1.48 ms                                                | 1.47 ms: 1.01x faster                                                            |
| xml_etree_generate         | 89.2 ms                                                | 88.8 ms: 1.00x faster                                                            |
| pidigits                   | 187 ms                                                 | 188 ms: 1.01x slower                                                             |
| scimark_lu                 | 118 ms                                                 | 119 ms: 1.01x slower                                                             |
| dulwich_log                | 68.5 ms                                                | 68.9 ms: 1.01x slower                                                            |
| asyncio_tcp                | 491 ms                                                 | 494 ms: 1.01x slower                                                             |
| meteor_contest             | 112 ms                                                 | 113 ms: 1.01x slower                                                             |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                           |
| pickle_dict                | 35.5 us                                                | 35.8 us: 1.01x slower                                                            |
| async_tree_none_tg         | 450 ms                                                 | 454 ms: 1.01x slower                                                             |
| bench_thread_pool          | 842 us                                                 | 850 us: 1.01x slower                                                             |
| unpickle_pure_python       | 230 us                                                 | 233 us: 1.01x slower                                                             |
| mdp                        | 2.63 sec                                               | 2.67 sec: 1.01x slower                                                           |
| regex_effbot               | 3.61 ms                                                | 3.66 ms: 1.01x slower                                                            |
| pycparser                  | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                           |
| tomli_loads                | 2.33 sec                                               | 2.37 sec: 1.02x slower                                                           |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 737 ms: 1.02x slower                                                             |
| crypto_pyaes               | 81.9 ms                                                | 83.2 ms: 1.02x slower                                                            |
| regex_compile              | 148 ms                                                 | 151 ms: 1.02x slower                                                             |
| sympy_expand               | 478 ms                                                 | 490 ms: 1.02x slower                                                             |
| sqlite_synth               | 2.83 us                                                | 2.90 us: 1.02x slower                                                            |
| json_dumps                 | 10.4 ms                                                | 10.6 ms: 1.03x slower                                                            |
| 2to3                       | 274 ms                                                 | 282 ms: 1.03x slower                                                             |
| async_tree_memoization_tg  | 575 ms                                                 | 591 ms: 1.03x slower                                                             |
| xml_etree_iterparse        | 107 ms                                                 | 110 ms: 1.03x slower                                                             |
| logging_silent             | 104 ns                                                 | 107 ns: 1.03x slower                                                             |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                           |
| sqlglot_normalize          | 110 ms                                                 | 114 ms: 1.03x slower                                                             |
| pickle_list                | 5.08 us                                                | 5.26 us: 1.03x slower                                                            |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.04x slower                                                           |
| pprint_safe_repr           | 776 ms                                                 | 811 ms: 1.05x slower                                                             |
| fannkuch                   | 417 ms                                                 | 437 ms: 1.05x slower                                                             |
| pyflate                    | 482 ms                                                 | 508 ms: 1.05x slower                                                             |
| sqlglot_optimize           | 54.8 ms                                                | 57.7 ms: 1.05x slower                                                            |
| python_startup             | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                            |
| scimark_monte_carlo        | 75.1 ms                                                | 79.9 ms: 1.06x slower                                                            |
| richards                   | 45.8 ms                                                | 48.9 ms: 1.07x slower                                                            |
| regex_dna                  | 212 ms                                                 | 227 ms: 1.07x slower                                                             |
| pprint_pformat             | 1.57 sec                                               | 1.69 sec: 1.08x slower                                                           |
| chaos                      | 67.0 ms                                                | 72.2 ms: 1.08x slower                                                            |
| richards_super             | 51.5 ms                                                | 55.7 ms: 1.08x slower                                                            |
| float                      | 84.7 ms                                                | 91.8 ms: 1.08x slower                                                            |
| regex_v8                   | 23.1 ms                                                | 25.2 ms: 1.09x slower                                                            |
| go                         | 139 ms                                                 | 156 ms: 1.12x slower                                                             |
| nqueens                    | 83.3 ms                                                | 95.0 ms: 1.14x slower                                                            |
| mako                       | 11.9 ms                                                | 13.6 ms: 1.14x slower                                                            |
| scimark_fft                | 382 ms                                                 | 441 ms: 1.15x slower                                                             |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.84 ms: 1.16x slower                                                            |
| nbody                      | 97.0 ms                                                | 114 ms: 1.17x slower                                                             |
| telco                      | 7.10 ms                                                | 8.57 ms: 1.21x slower                                                            |
| deltablue                  | 3.72 ms                                                | 4.53 ms: 1.22x slower                                                            |
| spectral_norm              | 115 ms                                                 | 143 ms: 1.24x slower                                                             |
| python_startup_no_site     | 6.94 ms                                                | 8.74 ms: 1.26x slower                                                            |
| hexiom                     | 6.41 ms                                                | 8.24 ms: 1.28x slower                                                            |
| coverage                   | 72.7 ms                                                | 95.4 ms: 1.31x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (7): dask, async_tree_cpu_io_mixed, async_tree_memoization, bench_mp_pool, json, asyncio_websockets, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.99% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.93x