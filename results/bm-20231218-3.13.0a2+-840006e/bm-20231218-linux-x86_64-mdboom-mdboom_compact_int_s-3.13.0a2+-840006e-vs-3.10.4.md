
# Results vs. 3.10.4

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 840006e
- commit date: 2023-12-18
- overall geometric mean: 1.34x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.28x faster
- Memory change: 1.05x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 266 ms: 1.31x faster                                                   |
| chameleon      | 9.68 ms                                                | 7.08 ms: 1.37x faster                                                  |
| docutils       | 3.30 sec                                               | 2.60 sec: 1.27x faster                                                 |
| tornado_http   | 136 ms                                                 | 95.2 ms: 1.43x faster                                                  |
| Geometric mean | (ref)                                                  | 1.34x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 438 ms: 1.66x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 561 ms: 1.55x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 831 ms: 1.22x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.47x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 89.2 ms: 1.72x faster                                                  |
| float          | 117 ms                                                 | 81.9 ms: 1.43x faster                                                  |
| pidigits       | 191 ms                                                 | 288 ms: 1.51x slower                                                   |
| Geometric mean | (ref)                                                  | 1.18x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 135 ms: 1.39x faster                                                   |
| regex_v8       | 27.8 ms                                                | 24.9 ms: 1.11x faster                                                  |
| regex_effbot   | 3.63 ms                                                | 3.52 ms: 1.03x faster                                                  |
| regex_dna      | 227 ms                                                 | 220 ms: 1.03x faster                                                   |
| Geometric mean | (ref)                                                  | 1.13x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 305 us: 1.59x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 222 us: 1.49x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.13 sec: 1.47x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 59.1 ms: 1.34x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 86.5 ms: 1.15x faster                                                  |
| json_loads           | 31.2 us                                                | 28.2 us: 1.11x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                   |
| unpickle_list        | 5.20 us                                                | 4.87 us: 1.07x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                                   |
| unpickle             | 14.4 us                                                | 14.9 us: 1.03x slower                                                  |
| pickle               | 10.7 us                                                | 11.2 us: 1.05x slower                                                  |
| pickle_list          | 5.08 us                                                | 5.33 us: 1.05x slower                                                  |
| pickle_dict          | 29.6 us                                                | 35.3 us: 1.19x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.4 ms: 1.41x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.99 ms: 1.52x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.4 ms: 1.44x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 116 us: 4.71x faster                                                   |
| generators               | 80.1 ms                                                | 29.0 ms: 2.76x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.34 ms: 2.37x faster                                                  |
| chaos                    | 115 ms                                                 | 60.3 ms: 1.91x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 486 ms: 1.90x faster                                                   |
| raytrace                 | 507 ms                                                 | 279 ms: 1.82x faster                                                   |
| logging_silent           | 190 ns                                                 | 107 ns: 1.78x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 72.7 ms: 1.76x faster                                                  |
| comprehensions           | 28.8 us                                                | 16.4 us: 1.75x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 68.1 ms: 1.73x faster                                                  |
| richards_super           | 94.7 ms                                                | 54.7 ms: 1.73x faster                                                  |
| nbody                    | 154 ms                                                 | 89.2 ms: 1.72x faster                                                  |
| scimark_sor              | 220 ms                                                 | 128 ms: 1.72x faster                                                   |
| go                       | 240 ms                                                 | 141 ms: 1.70x faster                                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.28 ms: 1.70x faster                                                  |
| hexiom                   | 10.4 ms                                                | 6.25 ms: 1.66x faster                                                  |
| async_tree_none          | 728 ms                                                 | 438 ms: 1.66x faster                                                   |
| coroutines               | 35.1 ms                                                | 21.3 ms: 1.65x faster                                                  |
| richards                 | 79.3 ms                                                | 48.3 ms: 1.64x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.60 ms: 1.61x faster                                                  |
| pyflate                  | 716 ms                                                 | 448 ms: 1.60x faster                                                   |
| pickle_pure_python       | 484 us                                                 | 305 us: 1.59x faster                                                   |
| spectral_norm            | 170 ms                                                 | 108 ms: 1.57x faster                                                   |
| async_tree_memoization   | 870 ms                                                 | 561 ms: 1.55x faster                                                   |
| scimark_lu               | 176 ms                                                 | 117 ms: 1.51x faster                                                   |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                 |
| unpickle_pure_python     | 331 us                                                 | 222 us: 1.49x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 39.3 us: 1.49x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.13 sec: 1.47x faster                                                 |
| logging_format           | 9.09 us                                                | 6.28 us: 1.45x faster                                                  |
| logging_simple           | 8.30 us                                                | 5.76 us: 1.44x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.44x faster                                                 |
| mako                     | 16.3 ms                                                | 11.4 ms: 1.44x faster                                                  |
| tornado_http             | 136 ms                                                 | 95.2 ms: 1.43x faster                                                  |
| float                    | 117 ms                                                 | 81.9 ms: 1.43x faster                                                  |
| python_startup           | 14.6 ms                                                | 10.4 ms: 1.41x faster                                                  |
| regex_compile            | 188 ms                                                 | 135 ms: 1.39x faster                                                   |
| unpack_sequence          | 60.0 ns                                                | 43.3 ns: 1.39x faster                                                  |
| pprint_pformat           | 2.10 sec                                               | 1.53 sec: 1.38x faster                                                 |
| chameleon                | 9.68 ms                                                | 7.08 ms: 1.37x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                  |
| pprint_safe_repr         | 1.02 sec                                               | 749 ms: 1.36x faster                                                   |
| deepcopy                 | 479 us                                                 | 355 us: 1.35x faster                                                   |
| fannkuch                 | 532 ms                                                 | 394 ms: 1.35x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.17 sec: 1.35x faster                                                 |
| xml_etree_process        | 79.1 ms                                                | 59.1 ms: 1.34x faster                                                  |
| nqueens                  | 106 ms                                                 | 79.1 ms: 1.34x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 107 ms: 1.34x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.14 us: 1.33x faster                                                  |
| sympy_sum                | 196 ms                                                 | 148 ms: 1.33x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.32x faster                                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.91 ms: 1.32x faster                                                  |
| 2to3                     | 348 ms                                                 | 266 ms: 1.31x faster                                                   |
| scimark_fft              | 466 ms                                                 | 357 ms: 1.30x faster                                                   |
| dulwich_log              | 84.3 ms                                                | 65.5 ms: 1.29x faster                                                  |
| sqlglot_optimize         | 69.2 ms                                                | 54.1 ms: 1.28x faster                                                  |
| docutils                 | 3.30 sec                                               | 2.60 sec: 1.27x faster                                                 |
| sympy_str                | 346 ms                                                 | 273 ms: 1.27x faster                                                   |
| sympy_expand             | 566 ms                                                 | 456 ms: 1.24x faster                                                   |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 831 ms: 1.22x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 832 us: 1.19x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 86.5 ms: 1.15x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.0 ms: 1.14x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.51 sec: 1.13x faster                                                 |
| regex_v8                 | 27.8 ms                                                | 24.9 ms: 1.11x faster                                                  |
| json_loads               | 31.2 us                                                | 28.2 us: 1.11x faster                                                  |
| json                     | 5.69 ms                                                | 5.15 ms: 1.10x faster                                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                                  |
| meteor_contest           | 120 ms                                                 | 109 ms: 1.10x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.77 us: 1.09x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                   |
| unpickle_list            | 5.20 us                                                | 4.87 us: 1.07x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                                   |
| regex_effbot             | 3.63 ms                                                | 3.52 ms: 1.03x faster                                                  |
| regex_dna                | 227 ms                                                 | 220 ms: 1.03x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                   |
| gc_traversal             | 3.62 ms                                                | 3.59 ms: 1.01x faster                                                  |
| async_generators         | 444 ms                                                 | 453 ms: 1.02x slower                                                   |
| unpickle                 | 14.4 us                                                | 14.9 us: 1.03x slower                                                  |
| pickle                   | 10.7 us                                                | 11.2 us: 1.05x slower                                                  |
| pickle_list              | 5.08 us                                                | 5.33 us: 1.05x slower                                                  |
| telco                    | 7.27 ms                                                | 8.30 ms: 1.14x slower                                                  |
| coverage                 | 79.4 ms                                                | 93.7 ms: 1.18x slower                                                  |
| pickle_dict              | 29.6 us                                                | 35.3 us: 1.19x slower                                                  |
| pidigits                 | 191 ms                                                 | 288 ms: 1.51x slower                                                   |
| python_startup_no_site   | 5.93 ms                                                | 8.99 ms: 1.52x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.34x faster                                                           |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231218-3.13.0a2+-840006e/bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.31x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.28x


# Memory

- memory change: 1.05x