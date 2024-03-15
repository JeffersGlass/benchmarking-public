
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: 3342775
- commit date: 2024-01-03
- overall geometric mean: 1.01x slower
- HPT reliability: 96.40%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 278 ms: 1.01x slower                                           |
| chameleon      | 7.41 ms                                                | 7.20 ms: 1.03x faster                                          |
| docutils       | 2.77 sec                                               | 2.68 sec: 1.03x faster                                         |
| tornado_http   | 103 ms                                                 | 97.3 ms: 1.06x faster                                          |
| Geometric mean | (ref)                                                  | 1.03x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 443 ms: 1.06x faster                                           |
| async_tree_memoization    | 578 ms                                                 | 566 ms: 1.02x faster                                           |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 712 ms: 1.02x faster                                           |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.02x slower                                         |
| async_tree_memoization_tg | 575 ms                                                 | 589 ms: 1.03x slower                                           |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                         |
| Geometric mean            | (ref)                                                  | 1.00x faster                                                   |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                           |
| float          | 84.7 ms                                                | 87.7 ms: 1.04x slower                                          |
| nbody          | 97.0 ms                                                | 104 ms: 1.07x slower                                           |
| Geometric mean | (ref)                                                  | 1.04x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 145 ms: 1.02x faster                                           |
| regex_dna      | 212 ms                                                 | 218 ms: 1.03x slower                                           |
| regex_v8       | 23.1 ms                                                | 25.6 ms: 1.11x slower                                          |
| Geometric mean | (ref)                                                  | 1.03x slower                                                   |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| unpickle             | 15.9 us                                                | 14.7 us: 1.08x faster                                          |
| pickle_pure_python   | 324 us                                                 | 303 us: 1.07x faster                                           |
| xml_etree_process    | 61.7 ms                                                | 59.4 ms: 1.04x faster                                          |
| tomli_loads          | 2.33 sec                                               | 2.26 sec: 1.03x faster                                         |
| xml_etree_generate   | 89.2 ms                                                | 87.4 ms: 1.02x faster                                          |
| pickle_dict          | 35.5 us                                                | 35.0 us: 1.01x faster                                          |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                           |
| unpickle_pure_python | 230 us                                                 | 228 us: 1.01x faster                                           |
| json_loads           | 28.5 us                                                | 28.3 us: 1.01x faster                                          |
| unpickle_list        | 5.29 us                                                | 5.32 us: 1.01x slower                                          |
| pickle_list          | 5.08 us                                                | 5.12 us: 1.01x slower                                          |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                          |
| xml_etree_iterparse  | 107 ms                                                 | 110 ms: 1.03x slower                                           |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                   |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                          |
| python_startup_no_site | 6.94 ms                                                | 8.88 ms: 1.28x slower                                          |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 12.9 ms: 1.08x slower                                          |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 114 us: 1.38x faster                                           |
| unpack_sequence           | 54.0 ns                                                | 47.4 ns: 1.14x faster                                          |
| logging_format            | 7.23 us                                                | 6.39 us: 1.13x faster                                          |
| logging_simple            | 6.46 us                                                | 5.75 us: 1.12x faster                                          |
| raytrace                  | 312 ms                                                 | 284 ms: 1.10x faster                                           |
| comprehensions            | 21.8 us                                                | 20.0 us: 1.09x faster                                          |
| unpickle                  | 15.9 us                                                | 14.7 us: 1.08x faster                                          |
| pickle_pure_python        | 324 us                                                 | 303 us: 1.07x faster                                           |
| deepcopy_reduce           | 3.35 us                                                | 3.13 us: 1.07x faster                                          |
| async_tree_none           | 472 ms                                                 | 443 ms: 1.06x faster                                           |
| gc_traversal              | 3.79 ms                                                | 3.58 ms: 1.06x faster                                          |
| tornado_http              | 103 ms                                                 | 97.3 ms: 1.06x faster                                          |
| generators                | 31.2 ms                                                | 29.6 ms: 1.06x faster                                          |
| sqlglot_parse             | 1.36 ms                                                | 1.30 ms: 1.05x faster                                          |
| deepcopy                  | 371 us                                                 | 354 us: 1.05x faster                                           |
| sympy_sum                 | 169 ms                                                 | 161 ms: 1.05x faster                                           |
| xml_etree_process         | 61.7 ms                                                | 59.4 ms: 1.04x faster                                          |
| sympy_str                 | 300 ms                                                 | 290 ms: 1.03x faster                                           |
| docutils                  | 2.77 sec                                               | 2.68 sec: 1.03x faster                                         |
| tomli_loads               | 2.33 sec                                               | 2.26 sec: 1.03x faster                                         |
| chameleon                 | 7.41 ms                                                | 7.20 ms: 1.03x faster                                          |
| async_generators          | 463 ms                                                 | 451 ms: 1.03x faster                                           |
| pathlib                   | 19.3 ms                                                | 18.8 ms: 1.03x faster                                          |
| sqlglot_transpile         | 1.68 ms                                                | 1.64 ms: 1.03x faster                                          |
| crypto_pyaes              | 81.9 ms                                                | 79.8 ms: 1.03x faster                                          |
| regex_compile             | 148 ms                                                 | 145 ms: 1.02x faster                                           |
| xml_etree_generate        | 89.2 ms                                                | 87.4 ms: 1.02x faster                                          |
| async_tree_memoization    | 578 ms                                                 | 566 ms: 1.02x faster                                           |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 712 ms: 1.02x faster                                           |
| scimark_lu                | 118 ms                                                 | 116 ms: 1.02x faster                                           |
| pickle_dict               | 35.5 us                                                | 35.0 us: 1.01x faster                                          |
| dask                      | 372 ms                                                 | 368 ms: 1.01x faster                                           |
| xml_etree_parse           | 159 ms                                                 | 158 ms: 1.01x faster                                           |
| unpickle_pure_python      | 230 us                                                 | 228 us: 1.01x faster                                           |
| sympy_integrate           | 21.4 ms                                                | 21.3 ms: 1.01x faster                                          |
| asyncio_tcp               | 491 ms                                                 | 488 ms: 1.01x faster                                           |
| json_loads                | 28.5 us                                                | 28.3 us: 1.01x faster                                          |
| meteor_contest            | 112 ms                                                 | 112 ms: 1.00x faster                                           |
| dulwich_log               | 68.5 ms                                                | 68.3 ms: 1.00x faster                                          |
| bench_thread_pool         | 842 us                                                 | 844 us: 1.00x slower                                           |
| pidigits                  | 187 ms                                                 | 188 ms: 1.00x slower                                           |
| unpickle_list             | 5.29 us                                                | 5.32 us: 1.01x slower                                          |
| pickle_list               | 5.08 us                                                | 5.12 us: 1.01x slower                                          |
| scimark_sor               | 129 ms                                                 | 130 ms: 1.01x slower                                           |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.80 sec: 1.01x slower                                         |
| json_dumps                | 10.4 ms                                                | 10.5 ms: 1.01x slower                                          |
| richards                  | 45.8 ms                                                | 46.4 ms: 1.01x slower                                          |
| 2to3                      | 274 ms                                                 | 278 ms: 1.01x slower                                           |
| sqlite_synth              | 2.83 us                                                | 2.88 us: 1.02x slower                                          |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.02x slower                                         |
| richards_super            | 51.5 ms                                                | 52.6 ms: 1.02x slower                                          |
| sympy_expand              | 478 ms                                                 | 489 ms: 1.02x slower                                           |
| async_tree_memoization_tg | 575 ms                                                 | 589 ms: 1.03x slower                                           |
| xml_etree_iterparse       | 107 ms                                                 | 110 ms: 1.03x slower                                           |
| scimark_fft               | 382 ms                                                 | 393 ms: 1.03x slower                                           |
| pycparser                 | 1.18 sec                                               | 1.21 sec: 1.03x slower                                         |
| regex_dna                 | 212 ms                                                 | 218 ms: 1.03x slower                                           |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                         |
| scimark_monte_carlo       | 75.1 ms                                                | 77.6 ms: 1.03x slower                                          |
| float                     | 84.7 ms                                                | 87.7 ms: 1.04x slower                                          |
| sqlglot_optimize          | 54.8 ms                                                | 56.8 ms: 1.04x slower                                          |
| pprint_safe_repr          | 776 ms                                                 | 811 ms: 1.05x slower                                           |
| logging_silent            | 104 ns                                                 | 110 ns: 1.05x slower                                           |
| pyflate                   | 482 ms                                                 | 514 ms: 1.07x slower                                           |
| python_startup            | 9.55 ms                                                | 10.2 ms: 1.07x slower                                          |
| chaos                     | 67.0 ms                                                | 71.7 ms: 1.07x slower                                          |
| fannkuch                  | 417 ms                                                 | 447 ms: 1.07x slower                                           |
| mdp                       | 2.63 sec                                               | 2.82 sec: 1.07x slower                                         |
| nbody                     | 97.0 ms                                                | 104 ms: 1.07x slower                                           |
| mako                      | 11.9 ms                                                | 12.9 ms: 1.08x slower                                          |
| pprint_pformat            | 1.57 sec                                               | 1.71 sec: 1.09x slower                                         |
| deltablue                 | 3.72 ms                                                | 4.08 ms: 1.10x slower                                          |
| go                        | 139 ms                                                 | 153 ms: 1.10x slower                                           |
| regex_v8                  | 23.1 ms                                                | 25.6 ms: 1.11x slower                                          |
| nqueens                   | 83.3 ms                                                | 92.6 ms: 1.11x slower                                          |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 5.88 ms: 1.16x slower                                          |
| telco                     | 7.10 ms                                                | 8.52 ms: 1.20x slower                                          |
| spectral_norm             | 115 ms                                                 | 140 ms: 1.22x slower                                           |
| python_startup_no_site    | 6.94 ms                                                | 8.88 ms: 1.28x slower                                          |
| hexiom                    | 6.41 ms                                                | 8.23 ms: 1.28x slower                                          |
| coverage                  | 72.7 ms                                                | 95.9 ms: 1.32x slower                                          |
| Geometric mean            | (ref)                                                  | 1.01x slower                                                   |

Benchmark hidden because not significant (12): json, pickle, async_tree_cpu_io_mixed_tg, bench_mp_pool, create_gc_cycles, deepcopy_memo, regex_effbot, asyncio_websockets, sqlglot_normalize, coroutines, async_tree_none_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 96.40% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.96x