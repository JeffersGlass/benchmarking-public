
# Results vs. 3.10.4

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 2f0a32b
- commit date: 2023-12-19
- overall geometric mean: 1.34x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.28x faster
- Memory change: 1.05x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 266 ms: 1.31x faster                                                   |
| chameleon      | 9.68 ms                                                | 7.07 ms: 1.37x faster                                                  |
| docutils       | 3.30 sec                                               | 2.61 sec: 1.26x faster                                                 |
| tornado_http   | 136 ms                                                 | 95.2 ms: 1.43x faster                                                  |
| Geometric mean | (ref)                                                  | 1.34x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 439 ms: 1.66x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 566 ms: 1.54x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 728 ms: 1.40x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.52x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 90.5 ms: 1.70x faster                                                  |
| float          | 117 ms                                                 | 82.4 ms: 1.42x faster                                                  |
| pidigits       | 191 ms                                                 | 228 ms: 1.19x slower                                                   |
| Geometric mean | (ref)                                                  | 1.26x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 135 ms: 1.40x faster                                                   |
| regex_v8       | 27.8 ms                                                | 25.7 ms: 1.08x faster                                                  |
| regex_dna      | 227 ms                                                 | 216 ms: 1.05x faster                                                   |
| Geometric mean | (ref)                                                  | 1.12x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 307 us: 1.58x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 224 us: 1.48x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.18 sec: 1.44x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 59.4 ms: 1.33x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 86.6 ms: 1.15x faster                                                  |
| json_loads           | 31.2 us                                                | 28.4 us: 1.10x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                   |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                                   |
| unpickle_list        | 5.20 us                                                | 4.93 us: 1.06x faster                                                  |
| pickle_list          | 5.08 us                                                | 4.98 us: 1.02x faster                                                  |
| unpickle             | 14.4 us                                                | 15.0 us: 1.05x slower                                                  |
| pickle               | 10.7 us                                                | 11.4 us: 1.07x slower                                                  |
| pickle_dict          | 29.6 us                                                | 34.1 us: 1.15x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.4 ms: 1.40x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 9.04 ms: 1.52x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.2 ms: 1.45x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 117 us: 4.67x faster                                                   |
| generators               | 80.1 ms                                                | 30.0 ms: 2.67x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.43 ms: 2.31x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 479 ms: 1.92x faster                                                   |
| chaos                    | 115 ms                                                 | 62.2 ms: 1.86x faster                                                  |
| raytrace                 | 507 ms                                                 | 274 ms: 1.85x faster                                                   |
| logging_silent           | 190 ns                                                 | 106 ns: 1.79x faster                                                   |
| scimark_sor              | 220 ms                                                 | 126 ms: 1.75x faster                                                   |
| richards_super           | 94.7 ms                                                | 54.5 ms: 1.74x faster                                                  |
| comprehensions           | 28.8 us                                                | 16.6 us: 1.73x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 68.5 ms: 1.72x faster                                                  |
| crypto_pyaes             | 128 ms                                                 | 74.4 ms: 1.72x faster                                                  |
| nbody                    | 154 ms                                                 | 90.5 ms: 1.70x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.29 ms: 1.68x faster                                                  |
| go                       | 240 ms                                                 | 143 ms: 1.67x faster                                                   |
| async_tree_none          | 728 ms                                                 | 439 ms: 1.66x faster                                                   |
| richards                 | 79.3 ms                                                | 47.9 ms: 1.65x faster                                                  |
| hexiom                   | 10.4 ms                                                | 6.36 ms: 1.63x faster                                                  |
| coroutines               | 35.1 ms                                                | 21.8 ms: 1.61x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.61 ms: 1.60x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 307 us: 1.58x faster                                                   |
| async_tree_memoization   | 870 ms                                                 | 566 ms: 1.54x faster                                                   |
| pyflate                  | 716 ms                                                 | 469 ms: 1.53x faster                                                   |
| scimark_lu               | 176 ms                                                 | 116 ms: 1.52x faster                                                   |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                 |
| spectral_norm            | 170 ms                                                 | 115 ms: 1.48x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 224 us: 1.48x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 39.9 us: 1.47x faster                                                  |
| mako                     | 16.3 ms                                                | 11.2 ms: 1.45x faster                                                  |
| logging_format           | 9.09 us                                                | 6.31 us: 1.44x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.44x faster                                                 |
| tomli_loads              | 3.14 sec                                               | 2.18 sec: 1.44x faster                                                 |
| logging_simple           | 8.30 us                                                | 5.79 us: 1.43x faster                                                  |
| tornado_http             | 136 ms                                                 | 95.2 ms: 1.43x faster                                                  |
| float                    | 117 ms                                                 | 82.4 ms: 1.42x faster                                                  |
| python_startup           | 14.6 ms                                                | 10.4 ms: 1.40x faster                                                  |
| regex_compile            | 188 ms                                                 | 135 ms: 1.40x faster                                                   |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 728 ms: 1.40x faster                                                   |
| pprint_pformat           | 2.10 sec                                               | 1.51 sec: 1.39x faster                                                 |
| pprint_safe_repr         | 1.02 sec                                               | 741 ms: 1.37x faster                                                   |
| chameleon                | 9.68 ms                                                | 7.07 ms: 1.37x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                  |
| deepcopy                 | 479 us                                                 | 356 us: 1.35x faster                                                   |
| sqlglot_normalize        | 143 ms                                                 | 107 ms: 1.34x faster                                                   |
| xml_etree_process        | 79.1 ms                                                | 59.4 ms: 1.33x faster                                                  |
| deepcopy_reduce          | 4.17 us                                                | 3.14 us: 1.33x faster                                                  |
| sympy_sum                | 196 ms                                                 | 148 ms: 1.33x faster                                                   |
| fannkuch                 | 532 ms                                                 | 401 ms: 1.33x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.32x faster                                                  |
| 2to3                     | 348 ms                                                 | 266 ms: 1.31x faster                                                   |
| nqueens                  | 106 ms                                                 | 81.7 ms: 1.30x faster                                                  |
| pycparser                | 1.58 sec                                               | 1.22 sec: 1.29x faster                                                 |
| unpack_sequence          | 60.0 ns                                                | 46.9 ns: 1.28x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 66.0 ms: 1.28x faster                                                  |
| sqlglot_optimize         | 69.2 ms                                                | 54.3 ms: 1.27x faster                                                  |
| sympy_str                | 346 ms                                                 | 273 ms: 1.27x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.61 sec: 1.26x faster                                                 |
| scimark_fft              | 466 ms                                                 | 371 ms: 1.26x faster                                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.17 ms: 1.25x faster                                                  |
| sympy_expand             | 566 ms                                                 | 460 ms: 1.23x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 834 us: 1.18x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 86.6 ms: 1.15x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.2 ms: 1.12x faster                                                  |
| json_loads               | 31.2 us                                                | 28.4 us: 1.10x faster                                                  |
| json                     | 5.69 ms                                                | 5.20 ms: 1.09x faster                                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.48 ms: 1.09x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.80 us: 1.08x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 25.7 ms: 1.08x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.64 sec: 1.08x faster                                                 |
| meteor_contest           | 120 ms                                                 | 111 ms: 1.08x faster                                                   |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                                   |
| unpickle_list            | 5.20 us                                                | 4.93 us: 1.06x faster                                                  |
| regex_dna                | 227 ms                                                 | 216 ms: 1.05x faster                                                   |
| pickle_list              | 5.08 us                                                | 4.98 us: 1.02x faster                                                  |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                   |
| async_generators         | 444 ms                                                 | 446 ms: 1.00x slower                                                   |
| unpickle                 | 14.4 us                                                | 15.0 us: 1.05x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 3.82 ms: 1.05x slower                                                  |
| pickle                   | 10.7 us                                                | 11.4 us: 1.07x slower                                                  |
| pickle_dict              | 29.6 us                                                | 34.1 us: 1.15x slower                                                  |
| telco                    | 7.27 ms                                                | 8.39 ms: 1.15x slower                                                  |
| pidigits                 | 191 ms                                                 | 228 ms: 1.19x slower                                                   |
| coverage                 | 79.4 ms                                                | 95.3 ms: 1.20x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 9.04 ms: 1.52x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.34x faster                                                           |

Benchmark hidden because not significant (3): mypy2, regex_effbot, bench_mp_pool
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231219-3.13.0a2+-2f0a32b/bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.30x
- 95% likely to have a speedup of 1.29x
- 99% likely to have a speedup of 1.28x


# Memory

- memory change: 1.05x