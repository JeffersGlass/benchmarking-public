
# Results vs. 3.10.4

- fork: mdboom
- ref: pystats_test2
- machine: linux-x86_64
- commit hash: 28e6201
- commit date: 2024-02-07
- overall geometric mean: 1.29x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 280 ms: 1.24x faster                                            |
| chameleon      | 9.68 ms                                                | 7.24 ms: 1.34x faster                                           |
| docutils       | 3.30 sec                                               | 2.70 sec: 1.22x faster                                          |
| tornado_http   | 136 ms                                                 | 98.7 ms: 1.38x faster                                           |
| Geometric mean | (ref)                                                  | 1.29x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 446 ms: 1.63x faster                                            |
| async_tree_memoization  | 870 ms                                                 | 571 ms: 1.52x faster                                            |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.49x faster                                          |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 720 ms: 1.41x faster                                            |
| Geometric mean          | (ref)                                                  | 1.51x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 115 ms: 1.34x faster                                            |
| float          | 117 ms                                                 | 89.7 ms: 1.31x faster                                           |
| pidigits       | 191 ms                                                 | 188 ms: 1.02x faster                                            |
| Geometric mean | (ref)                                                  | 1.21x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 147 ms: 1.28x faster                                            |
| regex_v8       | 27.8 ms                                                | 25.3 ms: 1.10x faster                                           |
| regex_dna      | 227 ms                                                 | 220 ms: 1.03x faster                                            |
| Geometric mean | (ref)                                                  | 1.10x faster                                                    |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 300 us: 1.61x faster                                            |
| unpickle_pure_python | 331 us                                                 | 233 us: 1.42x faster                                            |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                           |
| xml_etree_process    | 79.1 ms                                                | 60.2 ms: 1.32x faster                                           |
| tomli_loads          | 3.14 sec                                               | 2.54 sec: 1.24x faster                                          |
| xml_etree_generate   | 99.4 ms                                                | 88.0 ms: 1.13x faster                                           |
| json_loads           | 31.2 us                                                | 28.3 us: 1.10x faster                                           |
| xml_etree_iterparse  | 115 ms                                                 | 108 ms: 1.07x faster                                            |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                            |
| unpickle_list        | 5.20 us                                                | 4.97 us: 1.05x faster                                           |
| pickle_list          | 5.08 us                                                | 5.06 us: 1.00x faster                                           |
| pickle               | 10.7 us                                                | 11.7 us: 1.10x slower                                           |
| pickle_dict          | 29.6 us                                                | 34.0 us: 1.15x slower                                           |
| unpickle             | 14.4 us                                                | 17.1 us: 1.19x slower                                           |
| Geometric mean       | (ref)                                                  | 1.12x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                           |
| python_startup_no_site | 5.93 ms                                                | 8.77 ms: 1.48x slower                                           |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.1 ms: 1.25x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 116 us: 4.70x faster                                            |
| generators               | 80.1 ms                                                | 29.6 ms: 2.70x faster                                           |
| deltablue                | 7.91 ms                                                | 3.50 ms: 2.26x faster                                           |
| asyncio_tcp              | 922 ms                                                 | 489 ms: 1.89x faster                                            |
| logging_silent           | 190 ns                                                 | 101 ns: 1.87x faster                                            |
| scimark_sor              | 220 ms                                                 | 124 ms: 1.77x faster                                            |
| richards_super           | 94.7 ms                                                | 54.3 ms: 1.74x faster                                           |
| raytrace                 | 507 ms                                                 | 296 ms: 1.71x faster                                            |
| richards                 | 79.3 ms                                                | 48.4 ms: 1.64x faster                                           |
| sqlglot_parse            | 2.17 ms                                                | 1.32 ms: 1.64x faster                                           |
| async_tree_none          | 728 ms                                                 | 446 ms: 1.63x faster                                            |
| coroutines               | 35.1 ms                                                | 21.6 ms: 1.62x faster                                           |
| chaos                    | 115 ms                                                 | 71.3 ms: 1.62x faster                                           |
| pickle_pure_python       | 484 us                                                 | 300 us: 1.61x faster                                            |
| crypto_pyaes             | 128 ms                                                 | 80.3 ms: 1.59x faster                                           |
| sqlglot_transpile        | 2.57 ms                                                | 1.66 ms: 1.55x faster                                           |
| scimark_monte_carlo      | 118 ms                                                 | 77.5 ms: 1.52x faster                                           |
| async_tree_memoization   | 870 ms                                                 | 571 ms: 1.52x faster                                            |
| scimark_lu               | 176 ms                                                 | 116 ms: 1.52x faster                                            |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.49x faster                                          |
| deepcopy_memo            | 58.5 us                                                | 40.0 us: 1.46x faster                                           |
| unpack_sequence          | 60.0 ns                                                | 41.3 ns: 1.45x faster                                           |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                           |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                          |
| unpickle_pure_python     | 331 us                                                 | 233 us: 1.42x faster                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 720 ms: 1.41x faster                                            |
| comprehensions           | 28.8 us                                                | 20.4 us: 1.41x faster                                           |
| pyflate                  | 716 ms                                                 | 509 ms: 1.41x faster                                            |
| go                       | 240 ms                                                 | 172 ms: 1.39x faster                                            |
| logging_simple           | 8.30 us                                                | 5.96 us: 1.39x faster                                           |
| tornado_http             | 136 ms                                                 | 98.7 ms: 1.38x faster                                           |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                           |
| chameleon                | 9.68 ms                                                | 7.24 ms: 1.34x faster                                           |
| nbody                    | 154 ms                                                 | 115 ms: 1.34x faster                                            |
| deepcopy                 | 479 us                                                 | 358 us: 1.34x faster                                            |
| logging_format           | 9.09 us                                                | 6.80 us: 1.34x faster                                           |
| xml_etree_process        | 79.1 ms                                                | 60.2 ms: 1.32x faster                                           |
| float                    | 117 ms                                                 | 89.7 ms: 1.31x faster                                           |
| deepcopy_reduce          | 4.17 us                                                | 3.20 us: 1.30x faster                                           |
| pprint_safe_repr         | 1.02 sec                                               | 783 ms: 1.30x faster                                            |
| pprint_pformat           | 2.10 sec                                               | 1.62 sec: 1.30x faster                                          |
| hexiom                   | 10.4 ms                                                | 8.04 ms: 1.29x faster                                           |
| regex_compile            | 188 ms                                                 | 147 ms: 1.28x faster                                            |
| sqlglot_normalize        | 143 ms                                                 | 112 ms: 1.28x faster                                            |
| pycparser                | 1.58 sec                                               | 1.25 sec: 1.26x faster                                          |
| mako                     | 16.3 ms                                                | 13.1 ms: 1.25x faster                                           |
| 2to3                     | 348 ms                                                 | 280 ms: 1.24x faster                                            |
| spectral_norm            | 170 ms                                                 | 137 ms: 1.24x faster                                            |
| tomli_loads              | 3.14 sec                                               | 2.54 sec: 1.24x faster                                          |
| sympy_integrate          | 25.8 ms                                                | 21.0 ms: 1.23x faster                                           |
| fannkuch                 | 532 ms                                                 | 433 ms: 1.23x faster                                            |
| dulwich_log              | 84.3 ms                                                | 68.8 ms: 1.23x faster                                           |
| sympy_sum                | 196 ms                                                 | 160 ms: 1.23x faster                                            |
| docutils                 | 3.30 sec                                               | 2.70 sec: 1.22x faster                                          |
| sqlglot_optimize         | 69.2 ms                                                | 57.1 ms: 1.21x faster                                           |
| dask                     | 441 ms                                                 | 368 ms: 1.20x faster                                            |
| sympy_str                | 346 ms                                                 | 290 ms: 1.19x faster                                            |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.49 ms: 1.18x faster                                           |
| bench_thread_pool        | 986 us                                                 | 842 us: 1.17x faster                                            |
| sympy_expand             | 566 ms                                                 | 485 ms: 1.17x faster                                            |
| nqueens                  | 106 ms                                                 | 91.6 ms: 1.16x faster                                           |
| xml_etree_generate       | 99.4 ms                                                | 88.0 ms: 1.13x faster                                           |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                           |
| json_loads               | 31.2 us                                                | 28.3 us: 1.10x faster                                           |
| regex_v8                 | 27.8 ms                                                | 25.3 ms: 1.10x faster                                           |
| create_gc_cycles         | 1.62 ms                                                | 1.48 ms: 1.10x faster                                           |
| json                     | 5.69 ms                                                | 5.22 ms: 1.09x faster                                           |
| mdp                      | 2.85 sec                                               | 2.64 sec: 1.08x faster                                          |
| scimark_fft              | 466 ms                                                 | 432 ms: 1.08x faster                                            |
| xml_etree_iterparse      | 115 ms                                                 | 108 ms: 1.07x faster                                            |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                            |
| meteor_contest           | 120 ms                                                 | 113 ms: 1.06x faster                                            |
| sqlite_synth             | 3.02 us                                                | 2.86 us: 1.06x faster                                           |
| unpickle_list            | 5.20 us                                                | 4.97 us: 1.05x faster                                           |
| regex_dna                | 227 ms                                                 | 220 ms: 1.03x faster                                            |
| pidigits                 | 191 ms                                                 | 188 ms: 1.02x faster                                            |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                            |
| pickle_list              | 5.08 us                                                | 5.06 us: 1.00x faster                                           |
| async_generators         | 444 ms                                                 | 453 ms: 1.02x slower                                            |
| gc_traversal             | 3.62 ms                                                | 3.81 ms: 1.05x slower                                           |
| pickle                   | 10.7 us                                                | 11.7 us: 1.10x slower                                           |
| pickle_dict              | 29.6 us                                                | 34.0 us: 1.15x slower                                           |
| unpickle                 | 14.4 us                                                | 17.1 us: 1.19x slower                                           |
| telco                    | 7.27 ms                                                | 8.67 ms: 1.19x slower                                           |
| coverage                 | 79.4 ms                                                | 95.1 ms: 1.20x slower                                           |
| python_startup_no_site   | 5.93 ms                                                | 8.77 ms: 1.48x slower                                           |
| Geometric mean           | (ref)                                                  | 1.29x faster                                                    |

Benchmark hidden because not significant (3): mypy2, regex_effbot, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240207-3.13.0a3+-28e6201-PYTHON_UOPS/bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.23x
- 95% likely to have a speedup of 1.22x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.06x