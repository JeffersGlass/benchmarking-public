# Results vs. 3.12.0

- fork: python
- ref: cbf3d38cbeb6e640d595
- machine: linux-x86_64
- commit hash: cbf3d38
- commit date: 2024-03-05
- overall geometric mean: 1.05x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 292 ms: 1.07x slower                                                   |
| chameleon      | 7.41 ms                                                | 6.84 ms: 1.08x faster                                                  |
| docutils       | 2.77 sec                                               | 2.82 sec: 1.02x slower                                                 |
| tornado_http   | 103 ms                                                 | 99.5 ms: 1.03x faster                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 444 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 717 ms: 1.01x faster                                                   |
| async_tree_memoization    | 578 ms                                                 | 572 ms: 1.01x faster                                                   |
| async_tree_none_tg        | 450 ms                                                 | 455 ms: 1.01x slower                                                   |
| async_tree_io_tg          | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                 |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                 |
| async_tree_memoization_tg | 575 ms                                                 | 602 ms: 1.05x slower                                                   |
| Geometric mean            | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                                   |
| float          | 84.7 ms                                                | 91.4 ms: 1.08x slower                                                  |
| nbody          | 97.0 ms                                                | 117 ms: 1.20x slower                                                   |
| Geometric mean | (ref)                                                  | 1.09x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.57 ms: 1.01x faster                                                  |
| regex_dna      | 212 ms                                                 | 221 ms: 1.04x slower                                                   |
| regex_v8       | 23.1 ms                                                | 25.3 ms: 1.09x slower                                                  |
| regex_compile  | 148 ms                                                 | 173 ms: 1.16x slower                                                   |
| Geometric mean | (ref)                                                  | 1.07x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 304 us: 1.06x faster                                                   |
| unpickle_list        | 5.29 us                                                | 4.99 us: 1.06x faster                                                  |
| json_loads           | 28.5 us                                                | 27.2 us: 1.05x faster                                                  |
| unpickle             | 15.9 us                                                | 15.3 us: 1.04x faster                                                  |
| pickle_dict          | 35.5 us                                                | 34.9 us: 1.02x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 60.8 ms: 1.02x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| xml_etree_generate   | 89.2 ms                                                | 88.8 ms: 1.00x faster                                                  |
| pickle               | 11.6 us                                                | 11.7 us: 1.01x slower                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 111 ms: 1.04x slower                                                   |
| tomli_loads          | 2.33 sec                                               | 2.45 sec: 1.05x slower                                                 |
| unpickle_pure_python | 230 us                                                 | 278 us: 1.21x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (2): pickle_list, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.83 ms: 1.27x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 13.0 ms: 1.09x slower                                                  |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 115 us: 1.37x faster                                                   |
| deepcopy_reduce           | 3.35 us                                                | 3.05 us: 1.10x faster                                                  |
| chameleon                 | 7.41 ms                                                | 6.84 ms: 1.08x faster                                                  |
| logging_simple            | 6.46 us                                                | 6.04 us: 1.07x faster                                                  |
| logging_format            | 7.23 us                                                | 6.79 us: 1.07x faster                                                  |
| pickle_pure_python        | 324 us                                                 | 304 us: 1.06x faster                                                   |
| async_tree_none           | 472 ms                                                 | 444 ms: 1.06x faster                                                   |
| unpickle_list             | 5.29 us                                                | 4.99 us: 1.06x faster                                                  |
| generators                | 31.2 ms                                                | 29.6 ms: 1.05x faster                                                  |
| coroutines                | 23.2 ms                                                | 22.1 ms: 1.05x faster                                                  |
| json_loads                | 28.5 us                                                | 27.2 us: 1.05x faster                                                  |
| comprehensions            | 21.8 us                                                | 20.8 us: 1.05x faster                                                  |
| logging_silent            | 104 ns                                                 | 100 ns: 1.04x faster                                                   |
| deepcopy                  | 371 us                                                 | 358 us: 1.04x faster                                                   |
| unpickle                  | 15.9 us                                                | 15.3 us: 1.04x faster                                                  |
| tornado_http              | 103 ms                                                 | 99.5 ms: 1.03x faster                                                  |
| json                      | 5.26 ms                                                | 5.10 ms: 1.03x faster                                                  |
| sympy_sum                 | 169 ms                                                 | 164 ms: 1.03x faster                                                   |
| pathlib                   | 19.3 ms                                                | 19.0 ms: 1.02x faster                                                  |
| asyncio_tcp               | 491 ms                                                 | 482 ms: 1.02x faster                                                   |
| pickle_dict               | 35.5 us                                                | 34.9 us: 1.02x faster                                                  |
| sympy_integrate           | 21.4 ms                                                | 21.1 ms: 1.02x faster                                                  |
| xml_etree_process         | 61.7 ms                                                | 60.8 ms: 1.02x faster                                                  |
| regex_effbot              | 3.61 ms                                                | 3.57 ms: 1.01x faster                                                  |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 717 ms: 1.01x faster                                                   |
| xml_etree_parse           | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| async_tree_memoization    | 578 ms                                                 | 572 ms: 1.01x faster                                                   |
| deltablue                 | 3.72 ms                                                | 3.68 ms: 1.01x faster                                                  |
| xml_etree_generate        | 89.2 ms                                                | 88.8 ms: 1.00x faster                                                  |
| pidigits                  | 187 ms                                                 | 188 ms: 1.00x slower                                                   |
| sqlglot_normalize         | 110 ms                                                 | 111 ms: 1.01x slower                                                   |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                 |
| pickle                    | 11.6 us                                                | 11.7 us: 1.01x slower                                                  |
| async_tree_none_tg        | 450 ms                                                 | 455 ms: 1.01x slower                                                   |
| bench_thread_pool         | 842 us                                                 | 853 us: 1.01x slower                                                   |
| mdp                       | 2.63 sec                                               | 2.67 sec: 1.02x slower                                                 |
| docutils                  | 2.77 sec                                               | 2.82 sec: 1.02x slower                                                 |
| meteor_contest            | 112 ms                                                 | 115 ms: 1.02x slower                                                   |
| create_gc_cycles          | 1.48 ms                                                | 1.51 ms: 1.02x slower                                                  |
| crypto_pyaes              | 81.9 ms                                                | 84.2 ms: 1.03x slower                                                  |
| sqlite_synth              | 2.83 us                                                | 2.91 us: 1.03x slower                                                  |
| async_tree_io_tg          | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                 |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                 |
| dulwich_log               | 68.5 ms                                                | 71.1 ms: 1.04x slower                                                  |
| sqlglot_transpile         | 1.68 ms                                                | 1.75 ms: 1.04x slower                                                  |
| xml_etree_iterparse       | 107 ms                                                 | 111 ms: 1.04x slower                                                   |
| regex_dna                 | 212 ms                                                 | 221 ms: 1.04x slower                                                   |
| sqlglot_parse             | 1.36 ms                                                | 1.42 ms: 1.04x slower                                                  |
| async_tree_memoization_tg | 575 ms                                                 | 602 ms: 1.05x slower                                                   |
| sympy_expand              | 478 ms                                                 | 502 ms: 1.05x slower                                                   |
| tomli_loads               | 2.33 sec                                               | 2.45 sec: 1.05x slower                                                 |
| gc_traversal              | 3.79 ms                                                | 4.03 ms: 1.06x slower                                                  |
| 2to3                      | 274 ms                                                 | 292 ms: 1.07x slower                                                   |
| python_startup            | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                  |
| float                     | 84.7 ms                                                | 91.4 ms: 1.08x slower                                                  |
| pprint_safe_repr          | 776 ms                                                 | 843 ms: 1.09x slower                                                   |
| raytrace                  | 312 ms                                                 | 340 ms: 1.09x slower                                                   |
| mako                      | 11.9 ms                                                | 13.0 ms: 1.09x slower                                                  |
| unpack_sequence           | 54.0 ns                                                | 58.9 ns: 1.09x slower                                                  |
| regex_v8                  | 23.1 ms                                                | 25.3 ms: 1.09x slower                                                  |
| sqlglot_optimize          | 54.8 ms                                                | 60.2 ms: 1.10x slower                                                  |
| chaos                     | 67.0 ms                                                | 73.6 ms: 1.10x slower                                                  |
| scimark_sor               | 129 ms                                                 | 142 ms: 1.10x slower                                                   |
| pycparser                 | 1.18 sec                                               | 1.31 sec: 1.11x slower                                                 |
| pprint_pformat            | 1.57 sec                                               | 1.75 sec: 1.11x slower                                                 |
| scimark_fft               | 382 ms                                                 | 433 ms: 1.13x slower                                                   |
| fannkuch                  | 417 ms                                                 | 473 ms: 1.14x slower                                                   |
| scimark_monte_carlo       | 75.1 ms                                                | 85.5 ms: 1.14x slower                                                  |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 5.85 ms: 1.16x slower                                                  |
| regex_compile             | 148 ms                                                 | 173 ms: 1.16x slower                                                   |
| nqueens                   | 83.3 ms                                                | 97.8 ms: 1.17x slower                                                  |
| spectral_norm             | 115 ms                                                 | 136 ms: 1.18x slower                                                   |
| richards_super            | 51.5 ms                                                | 61.2 ms: 1.19x slower                                                  |
| nbody                     | 97.0 ms                                                | 117 ms: 1.20x slower                                                   |
| richards                  | 45.8 ms                                                | 55.1 ms: 1.20x slower                                                  |
| unpickle_pure_python      | 230 us                                                 | 278 us: 1.21x slower                                                   |
| telco                     | 7.10 ms                                                | 8.62 ms: 1.21x slower                                                  |
| pyflate                   | 482 ms                                                 | 586 ms: 1.22x slower                                                   |
| go                        | 139 ms                                                 | 175 ms: 1.26x slower                                                   |
| python_startup_no_site    | 6.94 ms                                                | 8.83 ms: 1.27x slower                                                  |
| coverage                  | 72.7 ms                                                | 96.9 ms: 1.33x slower                                                  |
| scimark_lu                | 118 ms                                                 | 157 ms: 1.33x slower                                                   |
| hexiom                    | 6.41 ms                                                | 9.02 ms: 1.41x slower                                                  |
| dask                      | 372 ms                                                 | 536 ms: 1.44x slower                                                   |
| Geometric mean            | (ref)                                                  | 1.05x slower                                                           |

Benchmark hidden because not significant (9): sympy_str, bench_mp_pool, async_generators, pickle_list, asyncio_websockets, deepcopy_memo, json_dumps, async_tree_cpu_io_mixed_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.94x