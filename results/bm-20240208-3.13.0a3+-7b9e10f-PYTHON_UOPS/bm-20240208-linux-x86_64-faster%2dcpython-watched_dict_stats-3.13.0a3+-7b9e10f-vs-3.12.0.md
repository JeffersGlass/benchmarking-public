
# Results vs. 3.12.0

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: 7b9e10f
- commit date: 2024-02-08
- overall geometric mean: 1.01x slower \*
- HPT reliability: 99.37%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 282 ms: 1.03x slower                                                           |
| chameleon      | 7.41 ms                                                | 7.18 ms: 1.03x faster                                                          |
| docutils       | 2.77 sec                                               | 2.69 sec: 1.03x faster                                                         |
| tornado_http   | 103 ms                                                 | 98.7 ms: 1.04x faster                                                          |
| Geometric mean | (ref)                                                  | 1.02x faster                                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|---------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 448 ms: 1.05x faster                                                           |
| async_tree_none_tg        | 450 ms                                                 | 456 ms: 1.02x slower                                                           |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                         |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                         |
| async_tree_memoization_tg | 575 ms                                                 | 595 ms: 1.04x slower                                                           |
| Geometric mean            | (ref)                                                  | 1.01x slower                                                                   |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_memoization, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                                           |
| float          | 84.7 ms                                                | 88.5 ms: 1.04x slower                                                          |
| nbody          | 97.0 ms                                                | 115 ms: 1.19x slower                                                           |
| Geometric mean | (ref)                                                  | 1.07x slower                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.65 ms: 1.01x slower                                                          |
| regex_dna      | 212 ms                                                 | 222 ms: 1.05x slower                                                           |
| regex_v8       | 23.1 ms                                                | 25.0 ms: 1.08x slower                                                          |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                   |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 298 us: 1.09x faster                                                           |
| unpickle_list        | 5.29 us                                                | 4.99 us: 1.06x faster                                                          |
| unpickle             | 15.9 us                                                | 15.3 us: 1.03x faster                                                          |
| json_loads           | 28.5 us                                                | 27.7 us: 1.03x faster                                                          |
| xml_etree_process    | 61.7 ms                                                | 59.9 ms: 1.03x faster                                                          |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.02x faster                                                           |
| xml_etree_generate   | 89.2 ms                                                | 88.1 ms: 1.01x faster                                                          |
| pickle_dict          | 35.5 us                                                | 35.3 us: 1.01x faster                                                          |
| unpickle_pure_python | 230 us                                                 | 231 us: 1.01x slower                                                           |
| json_dumps           | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                          |
| xml_etree_iterparse  | 107 ms                                                 | 109 ms: 1.02x slower                                                           |
| pickle               | 11.6 us                                                | 11.9 us: 1.02x slower                                                          |
| pickle_list          | 5.08 us                                                | 5.28 us: 1.04x slower                                                          |
| tomli_loads          | 2.33 sec                                               | 2.54 sec: 1.09x slower                                                         |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                          |
| python_startup_no_site | 6.94 ms                                                | 8.83 ms: 1.27x slower                                                          |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 13.2 ms: 1.11x slower                                                          |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|---------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 114 us: 1.38x faster                                                           |
| unpack_sequence           | 54.0 ns                                                | 39.9 ns: 1.35x faster                                                          |
| gc_traversal              | 3.79 ms                                                | 3.49 ms: 1.09x faster                                                          |
| pickle_pure_python        | 324 us                                                 | 298 us: 1.09x faster                                                           |
| logging_simple            | 6.46 us                                                | 5.96 us: 1.08x faster                                                          |
| deepcopy_reduce           | 3.35 us                                                | 3.11 us: 1.08x faster                                                          |
| logging_format            | 7.23 us                                                | 6.76 us: 1.07x faster                                                          |
| generators                | 31.2 ms                                                | 29.3 ms: 1.07x faster                                                          |
| comprehensions            | 21.8 us                                                | 20.5 us: 1.06x faster                                                          |
| unpickle_list             | 5.29 us                                                | 4.99 us: 1.06x faster                                                          |
| pathlib                   | 19.3 ms                                                | 18.3 ms: 1.06x faster                                                          |
| deltablue                 | 3.72 ms                                                | 3.51 ms: 1.06x faster                                                          |
| raytrace                  | 312 ms                                                 | 295 ms: 1.06x faster                                                           |
| sympy_sum                 | 169 ms                                                 | 160 ms: 1.06x faster                                                           |
| async_tree_none           | 472 ms                                                 | 448 ms: 1.05x faster                                                           |
| scimark_sor               | 129 ms                                                 | 123 ms: 1.05x faster                                                           |
| deepcopy                  | 371 us                                                 | 354 us: 1.05x faster                                                           |
| coroutines                | 23.2 ms                                                | 22.1 ms: 1.05x faster                                                          |
| tornado_http              | 103 ms                                                 | 98.7 ms: 1.04x faster                                                          |
| unpickle                  | 15.9 us                                                | 15.3 us: 1.03x faster                                                          |
| chameleon                 | 7.41 ms                                                | 7.18 ms: 1.03x faster                                                          |
| json_loads                | 28.5 us                                                | 27.7 us: 1.03x faster                                                          |
| xml_etree_process         | 61.7 ms                                                | 59.9 ms: 1.03x faster                                                          |
| docutils                  | 2.77 sec                                               | 2.69 sec: 1.03x faster                                                         |
| scimark_lu                | 118 ms                                                 | 115 ms: 1.03x faster                                                           |
| deepcopy_memo             | 40.7 us                                                | 39.7 us: 1.03x faster                                                          |
| sqlglot_parse             | 1.36 ms                                                | 1.33 ms: 1.02x faster                                                          |
| logging_silent            | 104 ns                                                 | 102 ns: 1.02x faster                                                           |
| sympy_str                 | 300 ms                                                 | 294 ms: 1.02x faster                                                           |
| json                      | 5.26 ms                                                | 5.16 ms: 1.02x faster                                                          |
| sympy_integrate           | 21.4 ms                                                | 21.0 ms: 1.02x faster                                                          |
| xml_etree_parse           | 159 ms                                                 | 157 ms: 1.02x faster                                                           |
| xml_etree_generate        | 89.2 ms                                                | 88.1 ms: 1.01x faster                                                          |
| create_gc_cycles          | 1.48 ms                                                | 1.46 ms: 1.01x faster                                                          |
| async_generators          | 463 ms                                                 | 460 ms: 1.01x faster                                                           |
| sqlglot_transpile         | 1.68 ms                                                | 1.67 ms: 1.01x faster                                                          |
| mdp                       | 2.63 sec                                               | 2.62 sec: 1.01x faster                                                         |
| asyncio_tcp               | 491 ms                                                 | 488 ms: 1.01x faster                                                           |
| pickle_dict               | 35.5 us                                                | 35.3 us: 1.01x faster                                                          |
| pidigits                  | 187 ms                                                 | 188 ms: 1.00x slower                                                           |
| unpickle_pure_python      | 230 us                                                 | 231 us: 1.01x slower                                                           |
| sqlite_synth              | 2.83 us                                                | 2.86 us: 1.01x slower                                                          |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                         |
| regex_effbot              | 3.61 ms                                                | 3.65 ms: 1.01x slower                                                          |
| dulwich_log               | 68.5 ms                                                | 69.4 ms: 1.01x slower                                                          |
| async_tree_none_tg        | 450 ms                                                 | 456 ms: 1.02x slower                                                           |
| json_dumps                | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                          |
| xml_etree_iterparse       | 107 ms                                                 | 109 ms: 1.02x slower                                                           |
| pprint_safe_repr          | 776 ms                                                 | 790 ms: 1.02x slower                                                           |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                         |
| pickle                    | 11.6 us                                                | 11.9 us: 1.02x slower                                                          |
| 2to3                      | 274 ms                                                 | 282 ms: 1.03x slower                                                           |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                         |
| scimark_monte_carlo       | 75.1 ms                                                | 77.6 ms: 1.03x slower                                                          |
| sympy_expand              | 478 ms                                                 | 495 ms: 1.03x slower                                                           |
| async_tree_memoization_tg | 575 ms                                                 | 595 ms: 1.04x slower                                                           |
| pickle_list               | 5.08 us                                                | 5.28 us: 1.04x slower                                                          |
| fannkuch                  | 417 ms                                                 | 433 ms: 1.04x slower                                                           |
| pprint_pformat            | 1.57 sec                                               | 1.64 sec: 1.04x slower                                                         |
| float                     | 84.7 ms                                                | 88.5 ms: 1.04x slower                                                          |
| pyflate                   | 482 ms                                                 | 504 ms: 1.04x slower                                                           |
| regex_dna                 | 212 ms                                                 | 222 ms: 1.05x slower                                                           |
| sqlglot_normalize         | 110 ms                                                 | 116 ms: 1.05x slower                                                           |
| richards_super            | 51.5 ms                                                | 54.3 ms: 1.05x slower                                                          |
| richards                  | 45.8 ms                                                | 48.3 ms: 1.05x slower                                                          |
| chaos                     | 67.0 ms                                                | 70.6 ms: 1.05x slower                                                          |
| sqlglot_optimize          | 54.8 ms                                                | 58.0 ms: 1.06x slower                                                          |
| pycparser                 | 1.18 sec                                               | 1.25 sec: 1.06x slower                                                         |
| python_startup            | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                          |
| regex_v8                  | 23.1 ms                                                | 25.0 ms: 1.08x slower                                                          |
| tomli_loads               | 2.33 sec                                               | 2.54 sec: 1.09x slower                                                         |
| mako                      | 11.9 ms                                                | 13.2 ms: 1.11x slower                                                          |
| scimark_fft               | 382 ms                                                 | 425 ms: 1.11x slower                                                           |
| nqueens                   | 83.3 ms                                                | 93.5 ms: 1.12x slower                                                          |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 5.75 ms: 1.14x slower                                                          |
| nbody                     | 97.0 ms                                                | 115 ms: 1.19x slower                                                           |
| spectral_norm             | 115 ms                                                 | 137 ms: 1.20x slower                                                           |
| telco                     | 7.10 ms                                                | 8.76 ms: 1.23x slower                                                          |
| go                        | 139 ms                                                 | 172 ms: 1.23x slower                                                           |
| python_startup_no_site    | 6.94 ms                                                | 8.83 ms: 1.27x slower                                                          |
| hexiom                    | 6.41 ms                                                | 8.21 ms: 1.28x slower                                                          |
| coverage                  | 72.7 ms                                                | 94.7 ms: 1.30x slower                                                          |
| Geometric mean            | (ref)                                                  | 1.01x slower                                                                   |

Benchmark hidden because not significant (11): dask, async_tree_cpu_io_mixed, async_tree_memoization, bench_mp_pool, asyncio_websockets, regex_compile, bench_thread_pool, crypto_pyaes, meteor_contest, async_tree_cpu_io_mixed_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.37% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.93x