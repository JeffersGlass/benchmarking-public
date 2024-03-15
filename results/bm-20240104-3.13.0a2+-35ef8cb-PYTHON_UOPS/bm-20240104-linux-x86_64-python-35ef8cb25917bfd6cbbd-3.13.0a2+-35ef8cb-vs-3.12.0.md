
# Results vs. 3.12.0

- fork: python
- ref: 35ef8cb25917bfd6cbbd
- machine: linux-x86_64
- commit hash: 35ef8cb
- commit date: 2024-01-04
- overall geometric mean: 1.04x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 285 ms: 1.04x slower                                                   |
| chameleon      | 7.41 ms                                                | 7.27 ms: 1.02x faster                                                  |
| docutils       | 2.77 sec                                               | 2.72 sec: 1.02x faster                                                 |
| tornado_http   | 103 ms                                                 | 98.2 ms: 1.05x faster                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 456 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 737 ms: 1.02x slower                                                   |
| async_tree_none_tg         | 450 ms                                                 | 458 ms: 1.02x slower                                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 594 ms: 1.03x slower                                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.23 sec: 1.04x slower                                                 |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.05x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                           |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 190 ms: 1.01x slower                                                   |
| float          | 84.7 ms                                                | 94.0 ms: 1.11x slower                                                  |
| nbody          | 97.0 ms                                                | 126 ms: 1.30x slower                                                   |
| Geometric mean | (ref)                                                  | 1.14x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.63 ms: 1.00x slower                                                  |
| regex_compile  | 148 ms                                                 | 156 ms: 1.05x slower                                                   |
| regex_v8       | 23.1 ms                                                | 24.6 ms: 1.06x slower                                                  |
| regex_dna      | 212 ms                                                 | 227 ms: 1.07x slower                                                   |
| Geometric mean | (ref)                                                  | 1.05x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| unpickle             | 15.9 us                                                | 14.7 us: 1.08x faster                                                  |
| pickle_pure_python   | 324 us                                                 | 304 us: 1.07x faster                                                   |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.02x faster                                                   |
| json_loads           | 28.5 us                                                | 28.2 us: 1.01x faster                                                  |
| pickle_dict          | 35.5 us                                                | 35.1 us: 1.01x faster                                                  |
| pickle               | 11.6 us                                                | 11.6 us: 1.00x faster                                                  |
| pickle_list          | 5.08 us                                                | 5.13 us: 1.01x slower                                                  |
| json_dumps           | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                  |
| unpickle_list        | 5.29 us                                                | 5.39 us: 1.02x slower                                                  |
| xml_etree_generate   | 89.2 ms                                                | 90.9 ms: 1.02x slower                                                  |
| unpickle_pure_python | 230 us                                                 | 239 us: 1.04x slower                                                   |
| xml_etree_iterparse  | 107 ms                                                 | 113 ms: 1.06x slower                                                   |
| tomli_loads          | 2.33 sec                                               | 2.53 sec: 1.09x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (1): xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.77 ms: 1.26x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 14.7 ms: 1.23x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 117 us: 1.35x faster                                                   |
| unpack_sequence            | 54.0 ns                                                | 41.7 ns: 1.29x faster                                                  |
| unpickle                   | 15.9 us                                                | 14.7 us: 1.08x faster                                                  |
| generators                 | 31.2 ms                                                | 29.1 ms: 1.07x faster                                                  |
| pickle_pure_python         | 324 us                                                 | 304 us: 1.07x faster                                                   |
| logging_format             | 7.23 us                                                | 6.80 us: 1.06x faster                                                  |
| logging_simple             | 6.46 us                                                | 6.08 us: 1.06x faster                                                  |
| deepcopy_reduce            | 3.35 us                                                | 3.16 us: 1.06x faster                                                  |
| tornado_http               | 103 ms                                                 | 98.2 ms: 1.05x faster                                                  |
| async_tree_none            | 472 ms                                                 | 456 ms: 1.04x faster                                                   |
| sympy_sum                  | 169 ms                                                 | 163 ms: 1.03x faster                                                   |
| deepcopy                   | 371 us                                                 | 360 us: 1.03x faster                                                   |
| raytrace                   | 312 ms                                                 | 304 ms: 1.03x faster                                                   |
| coroutines                 | 23.2 ms                                                | 22.5 ms: 1.03x faster                                                  |
| async_generators           | 463 ms                                                 | 453 ms: 1.02x faster                                                   |
| pathlib                    | 19.3 ms                                                | 18.9 ms: 1.02x faster                                                  |
| chameleon                  | 7.41 ms                                                | 7.27 ms: 1.02x faster                                                  |
| docutils                   | 2.77 sec                                               | 2.72 sec: 1.02x faster                                                 |
| xml_etree_parse            | 159 ms                                                 | 157 ms: 1.02x faster                                                   |
| sqlglot_parse              | 1.36 ms                                                | 1.34 ms: 1.02x faster                                                  |
| dask                       | 372 ms                                                 | 367 ms: 1.01x faster                                                   |
| json_loads                 | 28.5 us                                                | 28.2 us: 1.01x faster                                                  |
| pickle_dict                | 35.5 us                                                | 35.1 us: 1.01x faster                                                  |
| create_gc_cycles           | 1.48 ms                                                | 1.47 ms: 1.01x faster                                                  |
| pickle                     | 11.6 us                                                | 11.6 us: 1.00x faster                                                  |
| regex_effbot               | 3.61 ms                                                | 3.63 ms: 1.00x slower                                                  |
| dulwich_log                | 68.5 ms                                                | 68.9 ms: 1.01x slower                                                  |
| asyncio_tcp                | 491 ms                                                 | 494 ms: 1.01x slower                                                   |
| scimark_lu                 | 118 ms                                                 | 119 ms: 1.01x slower                                                   |
| sympy_integrate            | 21.4 ms                                                | 21.6 ms: 1.01x slower                                                  |
| pickle_list                | 5.08 us                                                | 5.13 us: 1.01x slower                                                  |
| gc_traversal               | 3.79 ms                                                | 3.83 ms: 1.01x slower                                                  |
| pycparser                  | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                 |
| mdp                        | 2.63 sec                                               | 2.66 sec: 1.01x slower                                                 |
| pidigits                   | 187 ms                                                 | 190 ms: 1.01x slower                                                   |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.81 sec: 1.01x slower                                                 |
| bench_thread_pool          | 842 us                                                 | 854 us: 1.01x slower                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 737 ms: 1.02x slower                                                   |
| async_tree_none_tg         | 450 ms                                                 | 458 ms: 1.02x slower                                                   |
| json_dumps                 | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                  |
| unpickle_list              | 5.29 us                                                | 5.39 us: 1.02x slower                                                  |
| xml_etree_generate         | 89.2 ms                                                | 90.9 ms: 1.02x slower                                                  |
| scimark_sor                | 129 ms                                                 | 132 ms: 1.02x slower                                                   |
| sqlite_synth               | 2.83 us                                                | 2.92 us: 1.03x slower                                                  |
| deepcopy_memo              | 40.7 us                                                | 41.9 us: 1.03x slower                                                  |
| comprehensions             | 21.8 us                                                | 22.5 us: 1.03x slower                                                  |
| logging_silent             | 104 ns                                                 | 108 ns: 1.03x slower                                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 594 ms: 1.03x slower                                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.23 sec: 1.04x slower                                                 |
| 2to3                       | 274 ms                                                 | 285 ms: 1.04x slower                                                   |
| unpickle_pure_python       | 230 us                                                 | 239 us: 1.04x slower                                                   |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.05x slower                                                 |
| regex_compile              | 148 ms                                                 | 156 ms: 1.05x slower                                                   |
| sqlglot_normalize          | 110 ms                                                 | 116 ms: 1.05x slower                                                   |
| sympy_expand               | 478 ms                                                 | 505 ms: 1.06x slower                                                   |
| meteor_contest             | 112 ms                                                 | 119 ms: 1.06x slower                                                   |
| xml_etree_iterparse        | 107 ms                                                 | 113 ms: 1.06x slower                                                   |
| python_startup             | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| regex_v8                   | 23.1 ms                                                | 24.6 ms: 1.06x slower                                                  |
| crypto_pyaes               | 81.9 ms                                                | 87.4 ms: 1.07x slower                                                  |
| regex_dna                  | 212 ms                                                 | 227 ms: 1.07x slower                                                   |
| sqlglot_optimize           | 54.8 ms                                                | 58.9 ms: 1.07x slower                                                  |
| pprint_safe_repr           | 776 ms                                                 | 836 ms: 1.08x slower                                                   |
| richards                   | 45.8 ms                                                | 49.7 ms: 1.08x slower                                                  |
| tomli_loads                | 2.33 sec                                               | 2.53 sec: 1.09x slower                                                 |
| richards_super             | 51.5 ms                                                | 56.0 ms: 1.09x slower                                                  |
| pprint_pformat             | 1.57 sec                                               | 1.74 sec: 1.11x slower                                                 |
| float                      | 84.7 ms                                                | 94.0 ms: 1.11x slower                                                  |
| scimark_monte_carlo        | 75.1 ms                                                | 84.8 ms: 1.13x slower                                                  |
| chaos                      | 67.0 ms                                                | 76.0 ms: 1.13x slower                                                  |
| fannkuch                   | 417 ms                                                 | 477 ms: 1.14x slower                                                   |
| pyflate                    | 482 ms                                                 | 554 ms: 1.15x slower                                                   |
| go                         | 139 ms                                                 | 161 ms: 1.15x slower                                                   |
| nqueens                    | 83.3 ms                                                | 101 ms: 1.21x slower                                                   |
| mako                       | 11.9 ms                                                | 14.7 ms: 1.23x slower                                                  |
| scimark_fft                | 382 ms                                                 | 472 ms: 1.24x slower                                                   |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 6.30 ms: 1.25x slower                                                  |
| telco                      | 7.10 ms                                                | 8.88 ms: 1.25x slower                                                  |
| python_startup_no_site     | 6.94 ms                                                | 8.77 ms: 1.26x slower                                                  |
| coverage                   | 72.7 ms                                                | 94.7 ms: 1.30x slower                                                  |
| nbody                      | 97.0 ms                                                | 126 ms: 1.30x slower                                                   |
| deltablue                  | 3.72 ms                                                | 4.87 ms: 1.31x slower                                                  |
| spectral_norm              | 115 ms                                                 | 157 ms: 1.36x slower                                                   |
| hexiom                     | 6.41 ms                                                | 9.02 ms: 1.41x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (9): sqlglot_transpile, sympy_str, async_tree_cpu_io_mixed, json, asyncio_websockets, bench_mp_pool, xml_etree_process, async_tree_memoization, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.93x