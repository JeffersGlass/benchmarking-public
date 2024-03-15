
# Results vs. 3.12.0

- fork: python
- ref: 05a370abd6cdfe4b54be
- machine: linux-x86_64
- commit hash: 05a370a
- commit date: 2023-12-01
- overall geometric mean: 1.03x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 263 ms: 1.04x faster                                                   |
| chameleon      | 7.41 ms                                                | 7.00 ms: 1.06x faster                                                  |
| docutils       | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                 |
| tornado_http   | 103 ms                                                 | 94.3 ms: 1.09x faster                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 435 ms: 1.09x faster                                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 710 ms: 1.02x faster                                                   |
| async_tree_memoization     | 578 ms                                                 | 568 ms: 1.02x faster                                                   |
| async_tree_none_tg         | 450 ms                                                 | 457 ms: 1.02x slower                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 738 ms: 1.02x slower                                                   |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                 |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                 |
| async_tree_memoization_tg  | 575 ms                                                 | 598 ms: 1.04x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.00x slower                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 92.4 ms: 1.05x faster                                                  |
| float          | 84.7 ms                                                | 80.9 ms: 1.05x faster                                                  |
| pidigits       | 187 ms                                                 | 196 ms: 1.04x slower                                                   |
| Geometric mean | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 133 ms: 1.12x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.68 ms: 1.02x slower                                                  |
| regex_dna      | 212 ms                                                 | 219 ms: 1.03x slower                                                   |
| regex_v8       | 23.1 ms                                                | 25.7 ms: 1.11x slower                                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.14 sec: 1.09x faster                                                 |
| pickle_pure_python   | 324 us                                                 | 302 us: 1.07x faster                                                   |
| unpickle_pure_python | 230 us                                                 | 217 us: 1.06x faster                                                   |
| unpickle_list        | 5.29 us                                                | 5.04 us: 1.05x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 59.4 ms: 1.04x faster                                                  |
| pickle_dict          | 35.5 us                                                | 34.3 us: 1.04x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 86.6 ms: 1.03x faster                                                  |
| unpickle             | 15.9 us                                                | 15.5 us: 1.02x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.02x faster                                                   |
| xml_etree_iterparse  | 107 ms                                                 | 106 ms: 1.01x faster                                                   |
| json_loads           | 28.5 us                                                | 28.2 us: 1.01x faster                                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (3): json_dumps, pickle_list, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.4 ms: 1.09x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 9.01 ms: 1.30x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.19x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.4 ms: 1.05x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 117 us: 1.35x faster                                                   |
| comprehensions             | 21.8 us                                                | 16.3 us: 1.34x faster                                                  |
| unpack_sequence            | 54.0 ns                                                | 46.6 ns: 1.16x faster                                                  |
| crypto_pyaes               | 81.9 ms                                                | 70.9 ms: 1.15x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                                   |
| raytrace                   | 312 ms                                                 | 272 ms: 1.15x faster                                                   |
| logging_format             | 7.23 us                                                | 6.32 us: 1.14x faster                                                  |
| deltablue                  | 3.72 ms                                                | 3.25 ms: 1.14x faster                                                  |
| logging_simple             | 6.46 us                                                | 5.74 us: 1.12x faster                                                  |
| sympy_str                  | 300 ms                                                 | 267 ms: 1.12x faster                                                   |
| regex_compile              | 148 ms                                                 | 133 ms: 1.12x faster                                                   |
| sympy_integrate            | 21.4 ms                                                | 19.5 ms: 1.10x faster                                                  |
| chaos                      | 67.0 ms                                                | 60.9 ms: 1.10x faster                                                  |
| generators                 | 31.2 ms                                                | 28.6 ms: 1.09x faster                                                  |
| tornado_http               | 103 ms                                                 | 94.3 ms: 1.09x faster                                                  |
| tomli_loads                | 2.33 sec                                               | 2.14 sec: 1.09x faster                                                 |
| async_tree_none            | 472 ms                                                 | 435 ms: 1.09x faster                                                   |
| scimark_monte_carlo        | 75.1 ms                                                | 69.3 ms: 1.08x faster                                                  |
| deepcopy_reduce            | 3.35 us                                                | 3.09 us: 1.08x faster                                                  |
| sqlglot_parse              | 1.36 ms                                                | 1.26 ms: 1.08x faster                                                  |
| pickle_pure_python         | 324 us                                                 | 302 us: 1.07x faster                                                   |
| sqlglot_transpile          | 1.68 ms                                                | 1.57 ms: 1.07x faster                                                  |
| pathlib                    | 19.3 ms                                                | 18.1 ms: 1.07x faster                                                  |
| coroutines                 | 23.2 ms                                                | 21.7 ms: 1.07x faster                                                  |
| deepcopy                   | 371 us                                                 | 349 us: 1.06x faster                                                   |
| docutils                   | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                 |
| unpickle_pure_python       | 230 us                                                 | 217 us: 1.06x faster                                                   |
| sympy_expand               | 478 ms                                                 | 451 ms: 1.06x faster                                                   |
| chameleon                  | 7.41 ms                                                | 7.00 ms: 1.06x faster                                                  |
| fannkuch                   | 417 ms                                                 | 394 ms: 1.06x faster                                                   |
| hexiom                     | 6.41 ms                                                | 6.09 ms: 1.05x faster                                                  |
| pyflate                    | 482 ms                                                 | 459 ms: 1.05x faster                                                   |
| pprint_safe_repr           | 776 ms                                                 | 739 ms: 1.05x faster                                                   |
| nbody                      | 97.0 ms                                                | 92.4 ms: 1.05x faster                                                  |
| unpickle_list              | 5.29 us                                                | 5.04 us: 1.05x faster                                                  |
| float                      | 84.7 ms                                                | 80.9 ms: 1.05x faster                                                  |
| scimark_sor                | 129 ms                                                 | 123 ms: 1.05x faster                                                   |
| async_generators           | 463 ms                                                 | 443 ms: 1.05x faster                                                   |
| mako                       | 11.9 ms                                                | 11.4 ms: 1.05x faster                                                  |
| dulwich_log                | 68.5 ms                                                | 65.5 ms: 1.05x faster                                                  |
| sqlglot_normalize          | 110 ms                                                 | 105 ms: 1.05x faster                                                   |
| deepcopy_memo              | 40.7 us                                                | 39.0 us: 1.04x faster                                                  |
| 2to3                       | 274 ms                                                 | 263 ms: 1.04x faster                                                   |
| scimark_fft                | 382 ms                                                 | 366 ms: 1.04x faster                                                   |
| nqueens                    | 83.3 ms                                                | 80.0 ms: 1.04x faster                                                  |
| xml_etree_process          | 61.7 ms                                                | 59.4 ms: 1.04x faster                                                  |
| pprint_pformat             | 1.57 sec                                               | 1.51 sec: 1.04x faster                                                 |
| pickle_dict                | 35.5 us                                                | 34.3 us: 1.04x faster                                                  |
| dask                       | 372 ms                                                 | 360 ms: 1.03x faster                                                   |
| spectral_norm              | 115 ms                                                 | 112 ms: 1.03x faster                                                   |
| xml_etree_generate         | 89.2 ms                                                | 86.6 ms: 1.03x faster                                                  |
| mdp                        | 2.63 sec                                               | 2.56 sec: 1.03x faster                                                 |
| meteor_contest             | 112 ms                                                 | 109 ms: 1.03x faster                                                   |
| scimark_lu                 | 118 ms                                                 | 115 ms: 1.03x faster                                                   |
| unpickle                   | 15.9 us                                                | 15.5 us: 1.02x faster                                                  |
| sqlglot_optimize           | 54.8 ms                                                | 53.5 ms: 1.02x faster                                                  |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 710 ms: 1.02x faster                                                   |
| bench_thread_pool          | 842 us                                                 | 828 us: 1.02x faster                                                   |
| async_tree_memoization     | 578 ms                                                 | 568 ms: 1.02x faster                                                   |
| asyncio_tcp                | 491 ms                                                 | 483 ms: 1.02x faster                                                   |
| xml_etree_parse            | 159 ms                                                 | 157 ms: 1.02x faster                                                   |
| json                       | 5.26 ms                                                | 5.19 ms: 1.01x faster                                                  |
| xml_etree_iterparse        | 107 ms                                                 | 106 ms: 1.01x faster                                                   |
| json_loads                 | 28.5 us                                                | 28.2 us: 1.01x faster                                                  |
| sqlite_synth               | 2.83 us                                                | 2.81 us: 1.01x faster                                                  |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.02 ms: 1.01x faster                                                  |
| create_gc_cycles           | 1.48 ms                                                | 1.46 ms: 1.01x faster                                                  |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.78 sec: 1.00x faster                                                 |
| async_tree_none_tg         | 450 ms                                                 | 457 ms: 1.02x slower                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 738 ms: 1.02x slower                                                   |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                 |
| regex_effbot               | 3.61 ms                                                | 3.68 ms: 1.02x slower                                                  |
| pycparser                  | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| go                         | 139 ms                                                 | 142 ms: 1.02x slower                                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                 |
| regex_dna                  | 212 ms                                                 | 219 ms: 1.03x slower                                                   |
| richards_super             | 51.5 ms                                                | 53.3 ms: 1.04x slower                                                  |
| async_tree_memoization_tg  | 575 ms                                                 | 598 ms: 1.04x slower                                                   |
| pidigits                   | 187 ms                                                 | 196 ms: 1.04x slower                                                   |
| richards                   | 45.8 ms                                                | 47.9 ms: 1.04x slower                                                  |
| python_startup             | 9.55 ms                                                | 10.4 ms: 1.09x slower                                                  |
| gc_traversal               | 3.79 ms                                                | 4.16 ms: 1.10x slower                                                  |
| regex_v8                   | 23.1 ms                                                | 25.7 ms: 1.11x slower                                                  |
| telco                      | 7.10 ms                                                | 8.34 ms: 1.18x slower                                                  |
| python_startup_no_site     | 6.94 ms                                                | 9.01 ms: 1.30x slower                                                  |
| coverage                   | 72.7 ms                                                | 95.4 ms: 1.31x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (7): json_dumps, logging_silent, bench_mp_pool, asyncio_websockets, pickle_list, pickle, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.91x