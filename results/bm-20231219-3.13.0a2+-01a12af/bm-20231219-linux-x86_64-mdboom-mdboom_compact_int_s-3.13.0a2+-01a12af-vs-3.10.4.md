
# Results vs. 3.10.4

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 01a12af
- commit date: 2023-12-19
- overall geometric mean: 1.34x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.28x faster
- Memory change: 1.05x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 264 ms: 1.32x faster                                                   |
| chameleon      | 9.68 ms                                                | 7.01 ms: 1.38x faster                                                  |
| docutils       | 3.30 sec                                               | 2.61 sec: 1.26x faster                                                 |
| tornado_http   | 136 ms                                                 | 94.9 ms: 1.44x faster                                                  |
| Geometric mean | (ref)                                                  | 1.35x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 436 ms: 1.67x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 561 ms: 1.55x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 834 ms: 1.22x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.47x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 89.2 ms: 1.72x faster                                                  |
| float          | 117 ms                                                 | 81.5 ms: 1.44x faster                                                  |
| pidigits       | 191 ms                                                 | 289 ms: 1.51x slower                                                   |
| Geometric mean | (ref)                                                  | 1.18x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 136 ms: 1.39x faster                                                   |
| regex_v8       | 27.8 ms                                                | 24.5 ms: 1.13x faster                                                  |
| regex_dna      | 227 ms                                                 | 222 ms: 1.02x faster                                                   |
| regex_effbot   | 3.63 ms                                                | 3.69 ms: 1.02x slower                                                  |
| Geometric mean | (ref)                                                  | 1.12x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 306 us: 1.58x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 222 us: 1.49x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.17 sec: 1.45x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 59.4 ms: 1.33x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 86.2 ms: 1.15x faster                                                  |
| json_loads           | 31.2 us                                                | 28.2 us: 1.11x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                   |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                                   |
| pickle_list          | 5.08 us                                                | 5.15 us: 1.01x slower                                                  |
| unpickle             | 14.4 us                                                | 14.8 us: 1.03x slower                                                  |
| pickle               | 10.7 us                                                | 11.3 us: 1.06x slower                                                  |
| pickle_dict          | 29.6 us                                                | 32.8 us: 1.11x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.16x faster                                                           |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.4 ms: 1.41x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 9.00 ms: 1.52x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.2 ms: 1.46x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 117 us: 4.64x faster                                                   |
| generators               | 80.1 ms                                                | 29.3 ms: 2.73x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.30 ms: 2.40x faster                                                  |
| chaos                    | 115 ms                                                 | 60.6 ms: 1.90x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 485 ms: 1.90x faster                                                   |
| raytrace                 | 507 ms                                                 | 272 ms: 1.86x faster                                                   |
| logging_silent           | 190 ns                                                 | 105 ns: 1.81x faster                                                   |
| scimark_sor              | 220 ms                                                 | 123 ms: 1.78x faster                                                   |
| richards_super           | 94.7 ms                                                | 53.5 ms: 1.77x faster                                                  |
| crypto_pyaes             | 128 ms                                                 | 72.3 ms: 1.77x faster                                                  |
| comprehensions           | 28.8 us                                                | 16.5 us: 1.74x faster                                                  |
| nbody                    | 154 ms                                                 | 89.2 ms: 1.72x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 68.8 ms: 1.72x faster                                                  |
| hexiom                   | 10.4 ms                                                | 6.06 ms: 1.72x faster                                                  |
| go                       | 240 ms                                                 | 140 ms: 1.71x faster                                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.28 ms: 1.70x faster                                                  |
| richards                 | 79.3 ms                                                | 47.4 ms: 1.67x faster                                                  |
| async_tree_none          | 728 ms                                                 | 436 ms: 1.67x faster                                                   |
| sqlglot_transpile        | 2.57 ms                                                | 1.60 ms: 1.61x faster                                                  |
| coroutines               | 35.1 ms                                                | 21.9 ms: 1.60x faster                                                  |
| pyflate                  | 716 ms                                                 | 452 ms: 1.58x faster                                                   |
| pickle_pure_python       | 484 us                                                 | 306 us: 1.58x faster                                                   |
| async_tree_memoization   | 870 ms                                                 | 561 ms: 1.55x faster                                                   |
| spectral_norm            | 170 ms                                                 | 110 ms: 1.54x faster                                                   |
| scimark_lu               | 176 ms                                                 | 114 ms: 1.54x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 38.8 us: 1.51x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                 |
| unpickle_pure_python     | 331 us                                                 | 222 us: 1.49x faster                                                   |
| logging_simple           | 8.30 us                                                | 5.69 us: 1.46x faster                                                  |
| mako                     | 16.3 ms                                                | 11.2 ms: 1.46x faster                                                  |
| logging_format           | 9.09 us                                                | 6.25 us: 1.45x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.17 sec: 1.45x faster                                                 |
| tornado_http             | 136 ms                                                 | 94.9 ms: 1.44x faster                                                  |
| float                    | 117 ms                                                 | 81.5 ms: 1.44x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.44x faster                                                 |
| python_startup           | 14.6 ms                                                | 10.4 ms: 1.41x faster                                                  |
| pprint_pformat           | 2.10 sec                                               | 1.51 sec: 1.39x faster                                                 |
| regex_compile            | 188 ms                                                 | 136 ms: 1.39x faster                                                   |
| chameleon                | 9.68 ms                                                | 7.01 ms: 1.38x faster                                                  |
| pprint_safe_repr         | 1.02 sec                                               | 741 ms: 1.37x faster                                                   |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                  |
| pycparser                | 1.58 sec                                               | 1.16 sec: 1.36x faster                                                 |
| deepcopy                 | 479 us                                                 | 356 us: 1.35x faster                                                   |
| sqlglot_normalize        | 143 ms                                                 | 106 ms: 1.35x faster                                                   |
| fannkuch                 | 532 ms                                                 | 397 ms: 1.34x faster                                                   |
| sympy_sum                | 196 ms                                                 | 147 ms: 1.34x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.12 us: 1.34x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 59.4 ms: 1.33x faster                                                  |
| nqueens                  | 106 ms                                                 | 80.0 ms: 1.32x faster                                                  |
| sympy_integrate          | 25.8 ms                                                | 19.6 ms: 1.32x faster                                                  |
| 2to3                     | 348 ms                                                 | 264 ms: 1.32x faster                                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.01 ms: 1.29x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 65.4 ms: 1.29x faster                                                  |
| scimark_fft              | 466 ms                                                 | 362 ms: 1.29x faster                                                   |
| unpack_sequence          | 60.0 ns                                                | 46.7 ns: 1.29x faster                                                  |
| sympy_str                | 346 ms                                                 | 269 ms: 1.29x faster                                                   |
| sqlglot_optimize         | 69.2 ms                                                | 53.8 ms: 1.29x faster                                                  |
| docutils                 | 3.30 sec                                               | 2.61 sec: 1.26x faster                                                 |
| sympy_expand             | 566 ms                                                 | 455 ms: 1.24x faster                                                   |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 834 ms: 1.22x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 830 us: 1.19x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 86.2 ms: 1.15x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 24.5 ms: 1.13x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.2 ms: 1.12x faster                                                  |
| json                     | 5.69 ms                                                | 5.13 ms: 1.11x faster                                                  |
| json_loads               | 31.2 us                                                | 28.2 us: 1.11x faster                                                  |
| meteor_contest           | 120 ms                                                 | 109 ms: 1.10x faster                                                   |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                   |
| mdp                      | 2.85 sec                                               | 2.61 sec: 1.09x faster                                                 |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.08x faster                                                  |
| sqlite_synth             | 3.02 us                                                | 2.81 us: 1.08x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                                   |
| regex_dna                | 227 ms                                                 | 222 ms: 1.02x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                   |
| pickle_list              | 5.08 us                                                | 5.15 us: 1.01x slower                                                  |
| regex_effbot             | 3.63 ms                                                | 3.69 ms: 1.02x slower                                                  |
| unpickle                 | 14.4 us                                                | 14.8 us: 1.03x slower                                                  |
| pickle                   | 10.7 us                                                | 11.3 us: 1.06x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 3.96 ms: 1.09x slower                                                  |
| pickle_dict              | 29.6 us                                                | 32.8 us: 1.11x slower                                                  |
| telco                    | 7.27 ms                                                | 8.30 ms: 1.14x slower                                                  |
| coverage                 | 79.4 ms                                                | 94.2 ms: 1.19x slower                                                  |
| pidigits                 | 191 ms                                                 | 289 ms: 1.51x slower                                                   |
| python_startup_no_site   | 5.93 ms                                                | 9.00 ms: 1.52x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.34x faster                                                           |

Benchmark hidden because not significant (4): mypy2, unpickle_list, bench_mp_pool, async_generators
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231219-3.13.0a2+-01a12af/bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.31x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.28x


# Memory

- memory change: 1.05x