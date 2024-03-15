
# Results vs. 3.12.0

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: 1054202
- commit date: 2024-02-09
- overall geometric mean: 1.02x slower \*
- HPT reliability: 99.98%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 282 ms: 1.03x slower                                                           |
| docutils       | 2.77 sec                                               | 2.71 sec: 1.02x faster                                                         |
| tornado_http   | 103 ms                                                 | 98.6 ms: 1.04x faster                                                          |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                   |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 450 ms: 1.05x faster                                                           |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 733 ms: 1.01x slower                                                           |
| async_tree_none_tg         | 450 ms                                                 | 459 ms: 1.02x slower                                                           |
| async_tree_io_tg           | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                         |
| async_tree_memoization_tg  | 575 ms                                                 | 593 ms: 1.03x slower                                                           |
| async_tree_io              | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                         |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                                   |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                                           |
| float          | 84.7 ms                                                | 91.4 ms: 1.08x slower                                                          |
| nbody          | 97.0 ms                                                | 121 ms: 1.24x slower                                                           |
| Geometric mean | (ref)                                                  | 1.10x slower                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 150 ms: 1.01x slower                                                           |
| regex_effbot   | 3.61 ms                                                | 3.77 ms: 1.04x slower                                                          |
| regex_dna      | 212 ms                                                 | 228 ms: 1.07x slower                                                           |
| regex_v8       | 23.1 ms                                                | 25.1 ms: 1.09x slower                                                          |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 298 us: 1.09x faster                                                           |
| unpickle_list        | 5.29 us                                                | 5.03 us: 1.05x faster                                                          |
| unpickle             | 15.9 us                                                | 15.3 us: 1.04x faster                                                          |
| json_loads           | 28.5 us                                                | 27.7 us: 1.03x faster                                                          |
| pickle_dict          | 35.5 us                                                | 34.7 us: 1.02x faster                                                          |
| xml_etree_process    | 61.7 ms                                                | 60.6 ms: 1.02x faster                                                          |
| xml_etree_generate   | 89.2 ms                                                | 88.5 ms: 1.01x faster                                                          |
| unpickle_pure_python | 230 us                                                 | 232 us: 1.01x slower                                                           |
| json_dumps           | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                          |
| xml_etree_iterparse  | 107 ms                                                 | 109 ms: 1.02x slower                                                           |
| pickle_list          | 5.08 us                                                | 5.25 us: 1.03x slower                                                          |
| tomli_loads          | 2.33 sec                                               | 2.62 sec: 1.13x slower                                                         |
| Geometric mean       | (ref)                                                  | 1.00x faster                                                                   |

Benchmark hidden because not significant (2): xml_etree_parse, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                          |
| python_startup_no_site | 6.94 ms                                                | 8.75 ms: 1.26x slower                                                          |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 13.9 ms: 1.17x slower                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 115 us: 1.38x faster                                                           |
| pickle_pure_python         | 324 us                                                 | 298 us: 1.09x faster                                                           |
| logging_simple             | 6.46 us                                                | 6.03 us: 1.07x faster                                                          |
| deltablue                  | 3.72 ms                                                | 3.48 ms: 1.07x faster                                                          |
| scimark_sor                | 129 ms                                                 | 121 ms: 1.07x faster                                                           |
| logging_format             | 7.23 us                                                | 6.78 us: 1.07x faster                                                          |
| deepcopy_reduce            | 3.35 us                                                | 3.14 us: 1.07x faster                                                          |
| generators                 | 31.2 ms                                                | 29.4 ms: 1.06x faster                                                          |
| pathlib                    | 19.3 ms                                                | 18.4 ms: 1.05x faster                                                          |
| deepcopy                   | 371 us                                                 | 353 us: 1.05x faster                                                           |
| unpickle_list              | 5.29 us                                                | 5.03 us: 1.05x faster                                                          |
| raytrace                   | 312 ms                                                 | 298 ms: 1.05x faster                                                           |
| async_tree_none            | 472 ms                                                 | 450 ms: 1.05x faster                                                           |
| coroutines                 | 23.2 ms                                                | 22.1 ms: 1.05x faster                                                          |
| tornado_http               | 103 ms                                                 | 98.6 ms: 1.04x faster                                                          |
| unpickle                   | 15.9 us                                                | 15.3 us: 1.04x faster                                                          |
| sympy_sum                  | 169 ms                                                 | 163 ms: 1.04x faster                                                           |
| async_generators           | 463 ms                                                 | 449 ms: 1.03x faster                                                           |
| json                       | 5.26 ms                                                | 5.11 ms: 1.03x faster                                                          |
| logging_silent             | 104 ns                                                 | 101 ns: 1.03x faster                                                           |
| json_loads                 | 28.5 us                                                | 27.7 us: 1.03x faster                                                          |
| deepcopy_memo              | 40.7 us                                                | 39.7 us: 1.03x faster                                                          |
| pickle_dict                | 35.5 us                                                | 34.7 us: 1.02x faster                                                          |
| docutils                   | 2.77 sec                                               | 2.71 sec: 1.02x faster                                                         |
| sqlglot_parse              | 1.36 ms                                                | 1.33 ms: 1.02x faster                                                          |
| gc_traversal               | 3.79 ms                                                | 3.71 ms: 1.02x faster                                                          |
| scimark_lu                 | 118 ms                                                 | 116 ms: 1.02x faster                                                           |
| xml_etree_process          | 61.7 ms                                                | 60.6 ms: 1.02x faster                                                          |
| comprehensions             | 21.8 us                                                | 21.4 us: 1.02x faster                                                          |
| sympy_str                  | 300 ms                                                 | 294 ms: 1.02x faster                                                           |
| sqlglot_transpile          | 1.68 ms                                                | 1.67 ms: 1.01x faster                                                          |
| xml_etree_generate         | 89.2 ms                                                | 88.5 ms: 1.01x faster                                                          |
| sympy_integrate            | 21.4 ms                                                | 21.3 ms: 1.01x faster                                                          |
| asyncio_tcp                | 491 ms                                                 | 492 ms: 1.00x slower                                                           |
| pidigits                   | 187 ms                                                 | 188 ms: 1.00x slower                                                           |
| bench_thread_pool          | 842 us                                                 | 846 us: 1.00x slower                                                           |
| meteor_contest             | 112 ms                                                 | 113 ms: 1.01x slower                                                           |
| dulwich_log                | 68.5 ms                                                | 69.0 ms: 1.01x slower                                                          |
| unpickle_pure_python       | 230 us                                                 | 232 us: 1.01x slower                                                           |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 733 ms: 1.01x slower                                                           |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.81 sec: 1.01x slower                                                         |
| regex_compile              | 148 ms                                                 | 150 ms: 1.01x slower                                                           |
| sqlite_synth               | 2.83 us                                                | 2.88 us: 1.02x slower                                                          |
| json_dumps                 | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                          |
| async_tree_none_tg         | 450 ms                                                 | 459 ms: 1.02x slower                                                           |
| xml_etree_iterparse        | 107 ms                                                 | 109 ms: 1.02x slower                                                           |
| async_tree_io_tg           | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                         |
| 2to3                       | 274 ms                                                 | 282 ms: 1.03x slower                                                           |
| pprint_safe_repr           | 776 ms                                                 | 799 ms: 1.03x slower                                                           |
| async_tree_memoization_tg  | 575 ms                                                 | 593 ms: 1.03x slower                                                           |
| crypto_pyaes               | 81.9 ms                                                | 84.5 ms: 1.03x slower                                                          |
| pickle_list                | 5.08 us                                                | 5.25 us: 1.03x slower                                                          |
| async_tree_io              | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                         |
| sympy_expand               | 478 ms                                                 | 494 ms: 1.03x slower                                                           |
| pycparser                  | 1.18 sec                                               | 1.23 sec: 1.04x slower                                                         |
| sqlglot_normalize          | 110 ms                                                 | 115 ms: 1.04x slower                                                           |
| regex_effbot               | 3.61 ms                                                | 3.77 ms: 1.04x slower                                                          |
| fannkuch                   | 417 ms                                                 | 440 ms: 1.06x slower                                                           |
| pprint_pformat             | 1.57 sec                                               | 1.66 sec: 1.06x slower                                                         |
| unpack_sequence            | 54.0 ns                                                | 57.1 ns: 1.06x slower                                                          |
| python_startup             | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                          |
| sqlglot_optimize           | 54.8 ms                                                | 58.4 ms: 1.06x slower                                                          |
| regex_dna                  | 212 ms                                                 | 228 ms: 1.07x slower                                                           |
| richards                   | 45.8 ms                                                | 49.3 ms: 1.07x slower                                                          |
| float                      | 84.7 ms                                                | 91.4 ms: 1.08x slower                                                          |
| scimark_monte_carlo        | 75.1 ms                                                | 81.1 ms: 1.08x slower                                                          |
| richards_super             | 51.5 ms                                                | 55.7 ms: 1.08x slower                                                          |
| regex_v8                   | 23.1 ms                                                | 25.1 ms: 1.09x slower                                                          |
| pyflate                    | 482 ms                                                 | 526 ms: 1.09x slower                                                           |
| chaos                      | 67.0 ms                                                | 73.2 ms: 1.09x slower                                                          |
| go                         | 139 ms                                                 | 156 ms: 1.12x slower                                                           |
| tomli_loads                | 2.33 sec                                               | 2.62 sec: 1.13x slower                                                         |
| scimark_fft                | 382 ms                                                 | 440 ms: 1.15x slower                                                           |
| mako                       | 11.9 ms                                                | 13.9 ms: 1.17x slower                                                          |
| nqueens                    | 83.3 ms                                                | 97.6 ms: 1.17x slower                                                          |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 6.11 ms: 1.21x slower                                                          |
| telco                      | 7.10 ms                                                | 8.65 ms: 1.22x slower                                                          |
| nbody                      | 97.0 ms                                                | 121 ms: 1.24x slower                                                           |
| spectral_norm              | 115 ms                                                 | 144 ms: 1.25x slower                                                           |
| python_startup_no_site     | 6.94 ms                                                | 8.75 ms: 1.26x slower                                                          |
| coverage                   | 72.7 ms                                                | 94.8 ms: 1.30x slower                                                          |
| hexiom                     | 6.41 ms                                                | 8.44 ms: 1.32x slower                                                          |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                                   |

Benchmark hidden because not significant (11): xml_etree_parse, dask, async_tree_memoization, async_tree_cpu_io_mixed, chameleon, create_gc_cycles, bench_mp_pool, mdp, asyncio_websockets, pickle, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.98% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.93x