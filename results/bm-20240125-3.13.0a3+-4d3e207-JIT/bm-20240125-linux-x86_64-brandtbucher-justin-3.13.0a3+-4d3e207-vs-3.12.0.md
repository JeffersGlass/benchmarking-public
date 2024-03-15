
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: 4d3e207
- commit date: 2024-01-25
- overall geometric mean: 1.00x slower
- HPT reliability: 77.08%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 276 ms: 1.01x slower                                           |
| chameleon      | 7.41 ms                                                | 6.96 ms: 1.06x faster                                          |
| docutils       | 2.77 sec                                               | 2.66 sec: 1.04x faster                                         |
| tornado_http   | 103 ms                                                 | 97.4 ms: 1.05x faster                                          |
| Geometric mean | (ref)                                                  | 1.04x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 446 ms: 1.06x faster                                           |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 715 ms: 1.01x faster                                           |
| async_tree_none_tg        | 450 ms                                                 | 453 ms: 1.01x slower                                           |
| async_tree_io_tg          | 1.18 sec                                               | 1.20 sec: 1.02x slower                                         |
| async_tree_memoization_tg | 575 ms                                                 | 589 ms: 1.02x slower                                           |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                         |
| Geometric mean            | (ref)                                                  | 1.00x slower                                                   |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                           |
| float          | 84.7 ms                                                | 87.1 ms: 1.03x slower                                          |
| nbody          | 97.0 ms                                                | 104 ms: 1.07x slower                                           |
| Geometric mean | (ref)                                                  | 1.03x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 141 ms: 1.05x faster                                           |
| regex_effbot   | 3.61 ms                                                | 3.62 ms: 1.00x slower                                          |
| regex_dna      | 212 ms                                                 | 220 ms: 1.04x slower                                           |
| regex_v8       | 23.1 ms                                                | 25.5 ms: 1.10x slower                                          |
| Geometric mean | (ref)                                                  | 1.02x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|---------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_pure_python  | 324 us                                                 | 293 us: 1.10x faster                                           |
| tomli_loads         | 2.33 sec                                               | 2.20 sec: 1.06x faster                                         |
| pickle_dict         | 35.5 us                                                | 34.0 us: 1.05x faster                                          |
| xml_etree_process   | 61.7 ms                                                | 59.4 ms: 1.04x faster                                          |
| unpickle            | 15.9 us                                                | 15.5 us: 1.02x faster                                          |
| xml_etree_generate  | 89.2 ms                                                | 87.9 ms: 1.01x faster                                          |
| json_loads          | 28.5 us                                                | 28.2 us: 1.01x faster                                          |
| xml_etree_parse     | 159 ms                                                 | 158 ms: 1.01x faster                                           |
| json_dumps          | 10.4 ms                                                | 10.3 ms: 1.00x faster                                          |
| pickle              | 11.6 us                                                | 11.7 us: 1.01x slower                                          |
| unpickle_list       | 5.29 us                                                | 5.35 us: 1.01x slower                                          |
| xml_etree_iterparse | 107 ms                                                 | 109 ms: 1.02x slower                                           |
| pickle_list         | 5.08 us                                                | 5.23 us: 1.03x slower                                          |
| Geometric mean      | (ref)                                                  | 1.02x faster                                                   |

Benchmark hidden because not significant (1): unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                          |
| python_startup_no_site | 6.94 ms                                                | 8.82 ms: 1.27x slower                                          |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 12.7 ms: 1.07x slower                                          |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 111 us: 1.42x faster                                           |
| logging_format            | 7.23 us                                                | 6.37 us: 1.14x faster                                          |
| comprehensions            | 21.8 us                                                | 19.6 us: 1.11x faster                                          |
| logging_simple            | 6.46 us                                                | 5.81 us: 1.11x faster                                          |
| raytrace                  | 312 ms                                                 | 282 ms: 1.11x faster                                           |
| pickle_pure_python        | 324 us                                                 | 293 us: 1.10x faster                                           |
| unpack_sequence           | 54.0 ns                                                | 49.7 ns: 1.09x faster                                          |
| deepcopy_reduce           | 3.35 us                                                | 3.09 us: 1.08x faster                                          |
| generators                | 31.2 ms                                                | 29.2 ms: 1.07x faster                                          |
| chameleon                 | 7.41 ms                                                | 6.96 ms: 1.06x faster                                          |
| pathlib                   | 19.3 ms                                                | 18.2 ms: 1.06x faster                                          |
| deepcopy                  | 371 us                                                 | 350 us: 1.06x faster                                           |
| sqlglot_parse             | 1.36 ms                                                | 1.28 ms: 1.06x faster                                          |
| tomli_loads               | 2.33 sec                                               | 2.20 sec: 1.06x faster                                         |
| async_tree_none           | 472 ms                                                 | 446 ms: 1.06x faster                                           |
| tornado_http              | 103 ms                                                 | 97.4 ms: 1.05x faster                                          |
| sympy_sum                 | 169 ms                                                 | 160 ms: 1.05x faster                                           |
| regex_compile             | 148 ms                                                 | 141 ms: 1.05x faster                                           |
| sympy_str                 | 300 ms                                                 | 285 ms: 1.05x faster                                           |
| scimark_sor               | 129 ms                                                 | 123 ms: 1.05x faster                                           |
| pickle_dict               | 35.5 us                                                | 34.0 us: 1.05x faster                                          |
| sqlglot_transpile         | 1.68 ms                                                | 1.62 ms: 1.04x faster                                          |
| docutils                  | 2.77 sec                                               | 2.66 sec: 1.04x faster                                         |
| xml_etree_process         | 61.7 ms                                                | 59.4 ms: 1.04x faster                                          |
| deepcopy_memo             | 40.7 us                                                | 39.2 us: 1.04x faster                                          |
| scimark_lu                | 118 ms                                                 | 114 ms: 1.03x faster                                           |
| crypto_pyaes              | 81.9 ms                                                | 79.3 ms: 1.03x faster                                          |
| coroutines                | 23.2 ms                                                | 22.5 ms: 1.03x faster                                          |
| json                      | 5.26 ms                                                | 5.11 ms: 1.03x faster                                          |
| sympy_integrate           | 21.4 ms                                                | 20.9 ms: 1.03x faster                                          |
| async_generators          | 463 ms                                                 | 452 ms: 1.02x faster                                           |
| unpickle                  | 15.9 us                                                | 15.5 us: 1.02x faster                                          |
| meteor_contest            | 112 ms                                                 | 111 ms: 1.01x faster                                           |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 715 ms: 1.01x faster                                           |
| xml_etree_generate        | 89.2 ms                                                | 87.9 ms: 1.01x faster                                          |
| dask                      | 372 ms                                                 | 366 ms: 1.01x faster                                           |
| json_loads                | 28.5 us                                                | 28.2 us: 1.01x faster                                          |
| xml_etree_parse           | 159 ms                                                 | 158 ms: 1.01x faster                                           |
| dulwich_log               | 68.5 ms                                                | 67.9 ms: 1.01x faster                                          |
| scimark_monte_carlo       | 75.1 ms                                                | 74.6 ms: 1.01x faster                                          |
| bench_thread_pool         | 842 us                                                 | 837 us: 1.01x faster                                           |
| gc_traversal              | 3.79 ms                                                | 3.77 ms: 1.01x faster                                          |
| json_dumps                | 10.4 ms                                                | 10.3 ms: 1.00x faster                                          |
| asyncio_tcp               | 491 ms                                                 | 490 ms: 1.00x faster                                           |
| pidigits                  | 187 ms                                                 | 188 ms: 1.00x slower                                           |
| mdp                       | 2.63 sec                                               | 2.64 sec: 1.00x slower                                         |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.79 sec: 1.00x slower                                         |
| regex_effbot              | 3.61 ms                                                | 3.62 ms: 1.00x slower                                          |
| 2to3                      | 274 ms                                                 | 276 ms: 1.01x slower                                           |
| richards_super            | 51.5 ms                                                | 51.9 ms: 1.01x slower                                          |
| async_tree_none_tg        | 450 ms                                                 | 453 ms: 1.01x slower                                           |
| pickle                    | 11.6 us                                                | 11.7 us: 1.01x slower                                          |
| unpickle_list             | 5.29 us                                                | 5.35 us: 1.01x slower                                          |
| create_gc_cycles          | 1.48 ms                                                | 1.50 ms: 1.02x slower                                          |
| logging_silent            | 104 ns                                                 | 106 ns: 1.02x slower                                           |
| async_tree_io_tg          | 1.18 sec                                               | 1.20 sec: 1.02x slower                                         |
| pycparser                 | 1.18 sec                                               | 1.20 sec: 1.02x slower                                         |
| async_tree_memoization_tg | 575 ms                                                 | 589 ms: 1.02x slower                                           |
| xml_etree_iterparse       | 107 ms                                                 | 109 ms: 1.02x slower                                           |
| float                     | 84.7 ms                                                | 87.1 ms: 1.03x slower                                          |
| pickle_list               | 5.08 us                                                | 5.23 us: 1.03x slower                                          |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                         |
| sqlglot_optimize          | 54.8 ms                                                | 56.5 ms: 1.03x slower                                          |
| fannkuch                  | 417 ms                                                 | 433 ms: 1.04x slower                                           |
| regex_dna                 | 212 ms                                                 | 220 ms: 1.04x slower                                           |
| chaos                     | 67.0 ms                                                | 70.8 ms: 1.06x slower                                          |
| pyflate                   | 482 ms                                                 | 513 ms: 1.06x slower                                           |
| pprint_safe_repr          | 776 ms                                                 | 827 ms: 1.07x slower                                           |
| python_startup            | 9.55 ms                                                | 10.2 ms: 1.07x slower                                          |
| mako                      | 11.9 ms                                                | 12.7 ms: 1.07x slower                                          |
| nbody                     | 97.0 ms                                                | 104 ms: 1.07x slower                                           |
| go                        | 139 ms                                                 | 149 ms: 1.07x slower                                           |
| nqueens                   | 83.3 ms                                                | 89.9 ms: 1.08x slower                                          |
| pprint_pformat            | 1.57 sec                                               | 1.70 sec: 1.08x slower                                         |
| deltablue                 | 3.72 ms                                                | 4.05 ms: 1.09x slower                                          |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 5.55 ms: 1.10x slower                                          |
| regex_v8                  | 23.1 ms                                                | 25.5 ms: 1.10x slower                                          |
| telco                     | 7.10 ms                                                | 8.54 ms: 1.20x slower                                          |
| spectral_norm             | 115 ms                                                 | 141 ms: 1.23x slower                                           |
| hexiom                    | 6.41 ms                                                | 7.98 ms: 1.24x slower                                          |
| python_startup_no_site    | 6.94 ms                                                | 8.82 ms: 1.27x slower                                          |
| coverage                  | 72.7 ms                                                | 94.1 ms: 1.29x slower                                          |
| Geometric mean            | (ref)                                                  | 1.00x slower                                                   |

Benchmark hidden because not significant (11): async_tree_memoization, unpickle_pure_python, sqlglot_normalize, bench_mp_pool, scimark_fft, sqlite_synth, asyncio_websockets, sympy_expand, async_tree_cpu_io_mixed_tg, richards, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 77.08% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.96x