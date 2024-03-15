
# Results vs. 3.10.4

- fork: mdboom
- ref: compact_long
- machine: linux-x86_64
- commit hash: 39bbca4
- commit date: 2023-12-21
- overall geometric mean: 1.34x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.29x faster
- Memory change: 1.05x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 264 ms: 1.32x faster                                           |
| chameleon      | 9.68 ms                                                | 7.06 ms: 1.37x faster                                          |
| docutils       | 3.30 sec                                               | 2.59 sec: 1.27x faster                                         |
| tornado_http   | 136 ms                                                 | 95.0 ms: 1.44x faster                                          |
| Geometric mean | (ref)                                                  | 1.35x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 438 ms: 1.66x faster                                           |
| async_tree_memoization  | 870 ms                                                 | 565 ms: 1.54x faster                                           |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.49x faster                                         |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 727 ms: 1.40x faster                                           |
| Geometric mean          | (ref)                                                  | 1.52x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 91.2 ms: 1.68x faster                                          |
| float          | 117 ms                                                 | 81.9 ms: 1.43x faster                                          |
| pidigits       | 191 ms                                                 | 222 ms: 1.17x slower                                           |
| Geometric mean | (ref)                                                  | 1.27x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 134 ms: 1.40x faster                                           |
| regex_v8       | 27.8 ms                                                | 24.4 ms: 1.14x faster                                          |
| regex_dna      | 227 ms                                                 | 217 ms: 1.05x faster                                           |
| regex_effbot   | 3.63 ms                                                | 3.50 ms: 1.04x faster                                          |
| Geometric mean | (ref)                                                  | 1.15x faster                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 301 us: 1.61x faster                                           |
| unpickle_pure_python | 331 us                                                 | 220 us: 1.51x faster                                           |
| tomli_loads          | 3.14 sec                                               | 2.17 sec: 1.45x faster                                         |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                          |
| xml_etree_process    | 79.1 ms                                                | 59.0 ms: 1.34x faster                                          |
| xml_etree_generate   | 99.4 ms                                                | 85.9 ms: 1.16x faster                                          |
| json_loads           | 31.2 us                                                | 28.2 us: 1.11x faster                                          |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                           |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                           |
| unpickle_list        | 5.20 us                                                | 5.07 us: 1.03x faster                                          |
| pickle_list          | 5.08 us                                                | 5.05 us: 1.00x faster                                          |
| pickle               | 10.7 us                                                | 11.1 us: 1.04x slower                                          |
| unpickle             | 14.4 us                                                | 15.0 us: 1.04x slower                                          |
| pickle_dict          | 29.6 us                                                | 34.3 us: 1.16x slower                                          |
| Geometric mean       | (ref)                                                  | 1.16x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.4 ms: 1.41x faster                                          |
| python_startup_no_site | 5.93 ms                                                | 8.99 ms: 1.52x slower                                          |
| Geometric mean         | (ref)                                                  | 1.04x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.4 ms: 1.43x faster                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 118 us: 4.62x faster                                           |
| generators               | 80.1 ms                                                | 29.1 ms: 2.75x faster                                          |
| deltablue                | 7.91 ms                                                | 3.32 ms: 2.38x faster                                          |
| asyncio_tcp              | 922 ms                                                 | 485 ms: 1.90x faster                                           |
| chaos                    | 115 ms                                                 | 60.9 ms: 1.90x faster                                          |
| raytrace                 | 507 ms                                                 | 275 ms: 1.85x faster                                           |
| logging_silent           | 190 ns                                                 | 103 ns: 1.83x faster                                           |
| scimark_sor              | 220 ms                                                 | 124 ms: 1.78x faster                                           |
| richards_super           | 94.7 ms                                                | 53.7 ms: 1.76x faster                                          |
| comprehensions           | 28.8 us                                                | 16.3 us: 1.76x faster                                          |
| go                       | 240 ms                                                 | 139 ms: 1.73x faster                                           |
| scimark_monte_carlo      | 118 ms                                                 | 68.5 ms: 1.72x faster                                          |
| sqlglot_parse            | 2.17 ms                                                | 1.27 ms: 1.71x faster                                          |
| crypto_pyaes             | 128 ms                                                 | 75.0 ms: 1.70x faster                                          |
| hexiom                   | 10.4 ms                                                | 6.15 ms: 1.69x faster                                          |
| nbody                    | 154 ms                                                 | 91.2 ms: 1.68x faster                                          |
| async_tree_none          | 728 ms                                                 | 438 ms: 1.66x faster                                           |
| richards                 | 79.3 ms                                                | 47.7 ms: 1.66x faster                                          |
| sqlglot_transpile        | 2.57 ms                                                | 1.59 ms: 1.62x faster                                          |
| pickle_pure_python       | 484 us                                                 | 301 us: 1.61x faster                                           |
| coroutines               | 35.1 ms                                                | 22.5 ms: 1.56x faster                                          |
| async_tree_memoization   | 870 ms                                                 | 565 ms: 1.54x faster                                           |
| spectral_norm            | 170 ms                                                 | 111 ms: 1.54x faster                                           |
| pyflate                  | 716 ms                                                 | 472 ms: 1.52x faster                                           |
| scimark_lu               | 176 ms                                                 | 117 ms: 1.51x faster                                           |
| unpickle_pure_python     | 331 us                                                 | 220 us: 1.51x faster                                           |
| deepcopy_memo            | 58.5 us                                                | 39.2 us: 1.49x faster                                          |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.49x faster                                         |
| logging_simple           | 8.30 us                                                | 5.68 us: 1.46x faster                                          |
| logging_format           | 9.09 us                                                | 6.24 us: 1.46x faster                                          |
| tomli_loads              | 3.14 sec                                               | 2.17 sec: 1.45x faster                                         |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.44x faster                                         |
| tornado_http             | 136 ms                                                 | 95.0 ms: 1.44x faster                                          |
| float                    | 117 ms                                                 | 81.9 ms: 1.43x faster                                          |
| mako                     | 16.3 ms                                                | 11.4 ms: 1.43x faster                                          |
| python_startup           | 14.6 ms                                                | 10.4 ms: 1.41x faster                                          |
| regex_compile            | 188 ms                                                 | 134 ms: 1.40x faster                                           |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 727 ms: 1.40x faster                                           |
| pprint_pformat           | 2.10 sec                                               | 1.51 sec: 1.39x faster                                         |
| pycparser                | 1.58 sec                                               | 1.15 sec: 1.37x faster                                         |
| chameleon                | 9.68 ms                                                | 7.06 ms: 1.37x faster                                          |
| pprint_safe_repr         | 1.02 sec                                               | 745 ms: 1.37x faster                                           |
| deepcopy                 | 479 us                                                 | 351 us: 1.36x faster                                           |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                          |
| deepcopy_reduce          | 4.17 us                                                | 3.07 us: 1.36x faster                                          |
| sqlglot_normalize        | 143 ms                                                 | 106 ms: 1.35x faster                                           |
| fannkuch                 | 532 ms                                                 | 397 ms: 1.34x faster                                           |
| xml_etree_process        | 79.1 ms                                                | 59.0 ms: 1.34x faster                                          |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.85 ms: 1.34x faster                                          |
| sympy_sum                | 196 ms                                                 | 148 ms: 1.33x faster                                           |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.32x faster                                          |
| nqueens                  | 106 ms                                                 | 79.9 ms: 1.32x faster                                          |
| 2to3                     | 348 ms                                                 | 264 ms: 1.32x faster                                           |
| sympy_str                | 346 ms                                                 | 269 ms: 1.29x faster                                           |
| sqlglot_optimize         | 69.2 ms                                                | 53.8 ms: 1.29x faster                                          |
| dulwich_log              | 84.3 ms                                                | 65.8 ms: 1.28x faster                                          |
| docutils                 | 3.30 sec                                               | 2.59 sec: 1.27x faster                                         |
| scimark_fft              | 466 ms                                                 | 369 ms: 1.26x faster                                           |
| sympy_expand             | 566 ms                                                 | 457 ms: 1.24x faster                                           |
| bench_thread_pool        | 986 us                                                 | 827 us: 1.19x faster                                           |
| xml_etree_generate       | 99.4 ms                                                | 85.9 ms: 1.16x faster                                          |
| regex_v8                 | 27.8 ms                                                | 24.4 ms: 1.14x faster                                          |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                          |
| json_loads               | 31.2 us                                                | 28.2 us: 1.11x faster                                          |
| json                     | 5.69 ms                                                | 5.16 ms: 1.10x faster                                          |
| mdp                      | 2.85 sec                                               | 2.59 sec: 1.10x faster                                         |
| create_gc_cycles         | 1.62 ms                                                | 1.48 ms: 1.10x faster                                          |
| unpack_sequence          | 60.0 ns                                                | 54.7 ns: 1.10x faster                                          |
| meteor_contest           | 120 ms                                                 | 109 ms: 1.10x faster                                           |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                           |
| sqlite_synth             | 3.02 us                                                | 2.82 us: 1.07x faster                                          |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.06x faster                                           |
| regex_dna                | 227 ms                                                 | 217 ms: 1.05x faster                                           |
| regex_effbot             | 3.63 ms                                                | 3.50 ms: 1.04x faster                                          |
| unpickle_list            | 5.20 us                                                | 5.07 us: 1.03x faster                                          |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                           |
| async_generators         | 444 ms                                                 | 442 ms: 1.00x faster                                           |
| pickle_list              | 5.08 us                                                | 5.05 us: 1.00x faster                                          |
| pickle                   | 10.7 us                                                | 11.1 us: 1.04x slower                                          |
| unpickle                 | 14.4 us                                                | 15.0 us: 1.04x slower                                          |
| pickle_dict              | 29.6 us                                                | 34.3 us: 1.16x slower                                          |
| pidigits                 | 191 ms                                                 | 222 ms: 1.17x slower                                           |
| coverage                 | 79.4 ms                                                | 93.0 ms: 1.17x slower                                          |
| telco                    | 7.27 ms                                                | 8.55 ms: 1.18x slower                                          |
| gc_traversal             | 3.62 ms                                                | 4.30 ms: 1.19x slower                                          |
| python_startup_no_site   | 5.93 ms                                                | 8.99 ms: 1.52x slower                                          |
| Geometric mean           | (ref)                                                  | 1.34x faster                                                   |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231221-3.13.0a2+-39bbca4/bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.32x
- 95% likely to have a speedup of 1.31x
- 99% likely to have a speedup of 1.29x


# Memory

- memory change: 1.05x