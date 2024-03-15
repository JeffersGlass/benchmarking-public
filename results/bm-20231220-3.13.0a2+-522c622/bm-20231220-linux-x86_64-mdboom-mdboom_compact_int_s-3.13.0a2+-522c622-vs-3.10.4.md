
# Results vs. 3.10.4

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 522c622
- commit date: 2023-12-20
- overall geometric mean: 1.34x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.29x faster
- Memory change: 1.04x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 264 ms: 1.32x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.96 ms: 1.39x faster                                                  |
| docutils       | 3.30 sec                                               | 2.60 sec: 1.27x faster                                                 |
| tornado_http   | 136 ms                                                 | 95.1 ms: 1.43x faster                                                  |
| Geometric mean | (ref)                                                  | 1.35x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 436 ms: 1.67x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 562 ms: 1.55x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 729 ms: 1.39x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.52x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 89.7 ms: 1.71x faster                                                  |
| float          | 117 ms                                                 | 82.4 ms: 1.42x faster                                                  |
| pidigits       | 191 ms                                                 | 223 ms: 1.17x slower                                                   |
| Geometric mean | (ref)                                                  | 1.28x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 134 ms: 1.41x faster                                                   |
| regex_v8       | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                  |
| regex_dna      | 227 ms                                                 | 221 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.13x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 308 us: 1.57x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 223 us: 1.48x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.17 sec: 1.45x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 59.2 ms: 1.34x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 85.8 ms: 1.16x faster                                                  |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                   |
| unpickle_list        | 5.20 us                                                | 4.88 us: 1.06x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.05x faster                                                   |
| pickle_list          | 5.08 us                                                | 5.00 us: 1.01x faster                                                  |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                                  |
| pickle_dict          | 29.6 us                                                | 34.4 us: 1.16x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.16x faster                                                           |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.4 ms: 1.40x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 9.04 ms: 1.52x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.1 ms: 1.47x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 118 us: 4.62x faster                                                   |
| generators               | 80.1 ms                                                | 28.7 ms: 2.79x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.31 ms: 2.39x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 483 ms: 1.91x faster                                                   |
| chaos                    | 115 ms                                                 | 60.8 ms: 1.90x faster                                                  |
| raytrace                 | 507 ms                                                 | 272 ms: 1.86x faster                                                   |
| logging_silent           | 190 ns                                                 | 104 ns: 1.82x faster                                                   |
| scimark_sor              | 220 ms                                                 | 124 ms: 1.77x faster                                                   |
| comprehensions           | 28.8 us                                                | 16.4 us: 1.76x faster                                                  |
| richards_super           | 94.7 ms                                                | 54.0 ms: 1.75x faster                                                  |
| crypto_pyaes             | 128 ms                                                 | 73.3 ms: 1.74x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 68.8 ms: 1.72x faster                                                  |
| nbody                    | 154 ms                                                 | 89.7 ms: 1.71x faster                                                  |
| go                       | 240 ms                                                 | 140 ms: 1.71x faster                                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.28 ms: 1.70x faster                                                  |
| async_tree_none          | 728 ms                                                 | 436 ms: 1.67x faster                                                   |
| hexiom                   | 10.4 ms                                                | 6.23 ms: 1.67x faster                                                  |
| richards                 | 79.3 ms                                                | 48.2 ms: 1.65x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.60 ms: 1.61x faster                                                  |
| coroutines               | 35.1 ms                                                | 22.1 ms: 1.59x faster                                                  |
| pyflate                  | 716 ms                                                 | 455 ms: 1.57x faster                                                   |
| pickle_pure_python       | 484 us                                                 | 308 us: 1.57x faster                                                   |
| async_tree_memoization   | 870 ms                                                 | 562 ms: 1.55x faster                                                   |
| spectral_norm            | 170 ms                                                 | 111 ms: 1.52x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 38.7 us: 1.51x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                 |
| scimark_lu               | 176 ms                                                 | 118 ms: 1.50x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 223 us: 1.48x faster                                                   |
| mako                     | 16.3 ms                                                | 11.1 ms: 1.47x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.17 sec: 1.45x faster                                                 |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.45x faster                                                 |
| logging_simple           | 8.30 us                                                | 5.77 us: 1.44x faster                                                  |
| tornado_http             | 136 ms                                                 | 95.1 ms: 1.43x faster                                                  |
| logging_format           | 9.09 us                                                | 6.36 us: 1.43x faster                                                  |
| float                    | 117 ms                                                 | 82.4 ms: 1.42x faster                                                  |
| regex_compile            | 188 ms                                                 | 134 ms: 1.41x faster                                                   |
| pprint_pformat           | 2.10 sec                                               | 1.50 sec: 1.40x faster                                                 |
| python_startup           | 14.6 ms                                                | 10.4 ms: 1.40x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 729 ms: 1.39x faster                                                   |
| chameleon                | 9.68 ms                                                | 6.96 ms: 1.39x faster                                                  |
| pprint_safe_repr         | 1.02 sec                                               | 735 ms: 1.38x faster                                                   |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                  |
| deepcopy                 | 479 us                                                 | 351 us: 1.36x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.16 sec: 1.35x faster                                                 |
| sqlglot_normalize        | 143 ms                                                 | 107 ms: 1.34x faster                                                   |
| sympy_sum                | 196 ms                                                 | 147 ms: 1.34x faster                                                   |
| xml_etree_process        | 79.1 ms                                                | 59.2 ms: 1.34x faster                                                  |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.33x faster                                                  |
| deepcopy_reduce          | 4.17 us                                                | 3.15 us: 1.32x faster                                                  |
| fannkuch                 | 532 ms                                                 | 402 ms: 1.32x faster                                                   |
| 2to3                     | 348 ms                                                 | 264 ms: 1.32x faster                                                   |
| nqueens                  | 106 ms                                                 | 81.0 ms: 1.31x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 65.3 ms: 1.29x faster                                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.01 ms: 1.29x faster                                                  |
| sqlglot_optimize         | 69.2 ms                                                | 53.8 ms: 1.28x faster                                                  |
| sympy_str                | 346 ms                                                 | 271 ms: 1.28x faster                                                   |
| unpack_sequence          | 60.0 ns                                                | 47.2 ns: 1.27x faster                                                  |
| docutils                 | 3.30 sec                                               | 2.60 sec: 1.27x faster                                                 |
| scimark_fft              | 466 ms                                                 | 372 ms: 1.25x faster                                                   |
| sympy_expand             | 566 ms                                                 | 456 ms: 1.24x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 830 us: 1.19x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 85.8 ms: 1.16x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.2 ms: 1.12x faster                                                  |
| meteor_contest           | 120 ms                                                 | 108 ms: 1.11x faster                                                   |
| json_loads               | 31.2 us                                                | 28.1 us: 1.11x faster                                                  |
| json                     | 5.69 ms                                                | 5.13 ms: 1.11x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.09x faster                                                  |
| sqlite_synth             | 3.02 us                                                | 2.80 us: 1.08x faster                                                  |
| unpickle_list            | 5.20 us                                                | 4.88 us: 1.06x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.05x faster                                                   |
| mdp                      | 2.85 sec                                               | 2.77 sec: 1.03x faster                                                 |
| regex_dna                | 227 ms                                                 | 221 ms: 1.02x faster                                                   |
| pickle_list              | 5.08 us                                                | 5.00 us: 1.01x faster                                                  |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                   |
| async_generators         | 444 ms                                                 | 450 ms: 1.01x slower                                                   |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                                  |
| telco                    | 7.27 ms                                                | 8.36 ms: 1.15x slower                                                  |
| pickle_dict              | 29.6 us                                                | 34.4 us: 1.16x slower                                                  |
| pidigits                 | 191 ms                                                 | 223 ms: 1.17x slower                                                   |
| coverage                 | 79.4 ms                                                | 94.0 ms: 1.18x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 4.31 ms: 1.19x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 9.04 ms: 1.52x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.34x faster                                                           |

Benchmark hidden because not significant (4): mypy2, unpickle, bench_mp_pool, regex_effbot
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231220-3.13.0a2+-522c622/bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.31x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.29x


# Memory

- memory change: 1.04x