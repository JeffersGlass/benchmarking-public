
# Results vs. 3.12.0

- fork: python
- ref: a571a2fd3fdaeafdfd71
- machine: linux-x86_64
- commit hash: a571a2f
- commit date: 2024-01-18
- overall geometric mean: 1.05x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 264 ms: 1.04x faster                                                   |
| chameleon      | 7.41 ms                                                | 6.86 ms: 1.08x faster                                                  |
| docutils       | 2.77 sec                                               | 2.60 sec: 1.07x faster                                                 |
| tornado_http   | 103 ms                                                 | 94.5 ms: 1.09x faster                                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 432 ms: 1.09x faster                                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 703 ms: 1.03x faster                                                   |
| async_tree_memoization     | 578 ms                                                 | 560 ms: 1.03x faster                                                   |
| async_tree_none_tg         | 450 ms                                                 | 440 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 715 ms: 1.01x faster                                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.19 sec: 1.00x slower                                                 |
| async_tree_io              | 1.16 sec                                               | 1.17 sec: 1.01x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (1): async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 86.2 ms: 1.13x faster                                                  |
| float          | 84.7 ms                                                | 80.3 ms: 1.06x faster                                                  |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                                   |
| Geometric mean | (ref)                                                  | 1.06x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 129 ms: 1.15x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.63 ms: 1.00x slower                                                  |
| regex_dna      | 212 ms                                                 | 219 ms: 1.03x slower                                                   |
| regex_v8       | 23.1 ms                                                | 25.1 ms: 1.08x slower                                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.10 sec: 1.11x faster                                                 |
| pickle_pure_python   | 324 us                                                 | 296 us: 1.09x faster                                                   |
| unpickle_pure_python | 230 us                                                 | 213 us: 1.08x faster                                                   |
| unpickle             | 15.9 us                                                | 15.0 us: 1.05x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 58.8 ms: 1.05x faster                                                  |
| unpickle_list        | 5.29 us                                                | 5.04 us: 1.05x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 85.6 ms: 1.04x faster                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 104 ms: 1.02x faster                                                   |
| pickle_dict          | 35.5 us                                                | 34.8 us: 1.02x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| json_loads           | 28.5 us                                                | 28.3 us: 1.01x faster                                                  |
| json_dumps           | 10.4 ms                                                | 10.3 ms: 1.00x faster                                                  |
| pickle               | 11.6 us                                                | 11.7 us: 1.01x slower                                                  |
| pickle_list          | 5.08 us                                                | 5.17 us: 1.02x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.73 ms: 1.26x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.1 ms: 1.08x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-linux-x86_64-python-a571a2fd3fdaeafdfd71-3.13.0a3+-a571a2f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 109 us: 1.45x faster                                                   |
| comprehensions             | 21.8 us                                                | 16.1 us: 1.35x faster                                                  |
| unpack_sequence            | 54.0 ns                                                | 44.9 ns: 1.20x faster                                                  |
| raytrace                   | 312 ms                                                 | 260 ms: 1.20x faster                                                   |
| deltablue                  | 3.72 ms                                                | 3.21 ms: 1.16x faster                                                  |
| logging_format             | 7.23 us                                                | 6.27 us: 1.15x faster                                                  |
| crypto_pyaes               | 81.9 ms                                                | 71.1 ms: 1.15x faster                                                  |
| regex_compile              | 148 ms                                                 | 129 ms: 1.15x faster                                                   |
| chaos                      | 67.0 ms                                                | 58.5 ms: 1.14x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                                   |
| scimark_monte_carlo        | 75.1 ms                                                | 66.1 ms: 1.14x faster                                                  |
| logging_simple             | 6.46 us                                                | 5.70 us: 1.13x faster                                                  |
| nbody                      | 97.0 ms                                                | 86.2 ms: 1.13x faster                                                  |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.51 ms: 1.12x faster                                                  |
| tomli_loads                | 2.33 sec                                               | 2.10 sec: 1.11x faster                                                 |
| sympy_str                  | 300 ms                                                 | 270 ms: 1.11x faster                                                   |
| sympy_integrate            | 21.4 ms                                                | 19.5 ms: 1.10x faster                                                  |
| deepcopy_reduce            | 3.35 us                                                | 3.04 us: 1.10x faster                                                  |
| pickle_pure_python         | 324 us                                                 | 296 us: 1.09x faster                                                   |
| async_tree_none            | 472 ms                                                 | 432 ms: 1.09x faster                                                   |
| scimark_fft                | 382 ms                                                 | 350 ms: 1.09x faster                                                   |
| deepcopy_memo              | 40.7 us                                                | 37.4 us: 1.09x faster                                                  |
| sqlglot_parse              | 1.36 ms                                                | 1.25 ms: 1.09x faster                                                  |
| tornado_http               | 103 ms                                                 | 94.5 ms: 1.09x faster                                                  |
| deepcopy                   | 371 us                                                 | 342 us: 1.08x faster                                                   |
| chameleon                  | 7.41 ms                                                | 6.86 ms: 1.08x faster                                                  |
| unpickle_pure_python       | 230 us                                                 | 213 us: 1.08x faster                                                   |
| mako                       | 11.9 ms                                                | 11.1 ms: 1.08x faster                                                  |
| sqlglot_transpile          | 1.68 ms                                                | 1.57 ms: 1.07x faster                                                  |
| scimark_lu                 | 118 ms                                                 | 110 ms: 1.07x faster                                                   |
| spectral_norm              | 115 ms                                                 | 108 ms: 1.07x faster                                                   |
| pprint_safe_repr           | 776 ms                                                 | 728 ms: 1.07x faster                                                   |
| docutils                   | 2.77 sec                                               | 2.60 sec: 1.07x faster                                                 |
| pathlib                    | 19.3 ms                                                | 18.2 ms: 1.06x faster                                                  |
| generators                 | 31.2 ms                                                | 29.6 ms: 1.06x faster                                                  |
| pyflate                    | 482 ms                                                 | 457 ms: 1.06x faster                                                   |
| float                      | 84.7 ms                                                | 80.3 ms: 1.06x faster                                                  |
| unpickle                   | 15.9 us                                                | 15.0 us: 1.05x faster                                                  |
| hexiom                     | 6.41 ms                                                | 6.09 ms: 1.05x faster                                                  |
| pprint_pformat             | 1.57 sec                                               | 1.49 sec: 1.05x faster                                                 |
| xml_etree_process          | 61.7 ms                                                | 58.8 ms: 1.05x faster                                                  |
| unpickle_list              | 5.29 us                                                | 5.04 us: 1.05x faster                                                  |
| dulwich_log                | 68.5 ms                                                | 65.5 ms: 1.05x faster                                                  |
| nqueens                    | 83.3 ms                                                | 79.6 ms: 1.05x faster                                                  |
| meteor_contest             | 112 ms                                                 | 107 ms: 1.05x faster                                                   |
| sympy_expand               | 478 ms                                                 | 458 ms: 1.04x faster                                                   |
| mdp                        | 2.63 sec                                               | 2.52 sec: 1.04x faster                                                 |
| fannkuch                   | 417 ms                                                 | 400 ms: 1.04x faster                                                   |
| logging_silent             | 104 ns                                                 | 100 ns: 1.04x faster                                                   |
| xml_etree_generate         | 89.2 ms                                                | 85.6 ms: 1.04x faster                                                  |
| 2to3                       | 274 ms                                                 | 264 ms: 1.04x faster                                                   |
| async_generators           | 463 ms                                                 | 446 ms: 1.04x faster                                                   |
| dask                       | 372 ms                                                 | 360 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 703 ms: 1.03x faster                                                   |
| async_tree_memoization     | 578 ms                                                 | 560 ms: 1.03x faster                                                   |
| sqlglot_normalize          | 110 ms                                                 | 108 ms: 1.03x faster                                                   |
| xml_etree_iterparse        | 107 ms                                                 | 104 ms: 1.02x faster                                                   |
| pickle_dict                | 35.5 us                                                | 34.8 us: 1.02x faster                                                  |
| async_tree_none_tg         | 450 ms                                                 | 440 ms: 1.02x faster                                                   |
| asyncio_tcp                | 491 ms                                                 | 481 ms: 1.02x faster                                                   |
| json                       | 5.26 ms                                                | 5.16 ms: 1.02x faster                                                  |
| coroutines                 | 23.2 ms                                                | 22.7 ms: 1.02x faster                                                  |
| scimark_sor                | 129 ms                                                 | 127 ms: 1.02x faster                                                   |
| bench_thread_pool          | 842 us                                                 | 828 us: 1.02x faster                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 715 ms: 1.01x faster                                                   |
| sqlglot_optimize           | 54.8 ms                                                | 54.1 ms: 1.01x faster                                                  |
| go                         | 139 ms                                                 | 138 ms: 1.01x faster                                                   |
| xml_etree_parse            | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| json_loads                 | 28.5 us                                                | 28.3 us: 1.01x faster                                                  |
| json_dumps                 | 10.4 ms                                                | 10.3 ms: 1.00x faster                                                  |
| pidigits                   | 187 ms                                                 | 187 ms: 1.00x faster                                                   |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.79 sec: 1.00x slower                                                 |
| regex_effbot               | 3.61 ms                                                | 3.63 ms: 1.00x slower                                                  |
| async_tree_io_tg           | 1.18 sec                                               | 1.19 sec: 1.00x slower                                                 |
| pickle                     | 11.6 us                                                | 11.7 us: 1.01x slower                                                  |
| create_gc_cycles           | 1.48 ms                                                | 1.49 ms: 1.01x slower                                                  |
| async_tree_io              | 1.16 sec                                               | 1.17 sec: 1.01x slower                                                 |
| gc_traversal               | 3.79 ms                                                | 3.86 ms: 1.02x slower                                                  |
| pickle_list                | 5.08 us                                                | 5.17 us: 1.02x slower                                                  |
| pycparser                  | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| regex_dna                  | 212 ms                                                 | 219 ms: 1.03x slower                                                   |
| richards                   | 45.8 ms                                                | 47.7 ms: 1.04x slower                                                  |
| richards_super             | 51.5 ms                                                | 53.7 ms: 1.04x slower                                                  |
| python_startup             | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| regex_v8                   | 23.1 ms                                                | 25.1 ms: 1.08x slower                                                  |
| telco                      | 7.10 ms                                                | 8.24 ms: 1.16x slower                                                  |
| python_startup_no_site     | 6.94 ms                                                | 8.73 ms: 1.26x slower                                                  |
| coverage                   | 72.7 ms                                                | 94.9 ms: 1.31x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                           |

Benchmark hidden because not significant (5): sqlite_synth, async_tree_memoization_tg, asyncio_websockets, bench_mp_pool, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.93x