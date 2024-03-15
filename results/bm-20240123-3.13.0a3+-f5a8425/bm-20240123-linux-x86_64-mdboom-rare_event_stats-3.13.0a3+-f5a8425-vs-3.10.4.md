
# Results vs. 3.10.4

- fork: mdboom
- ref: rare_event_stats
- machine: linux-x86_64
- commit hash: f5a8425
- commit date: 2024-01-23
- overall geometric mean: 1.36x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.29x faster
- Memory change: 1.05x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 263 ms: 1.33x faster                                               |
| chameleon      | 9.68 ms                                                | 6.87 ms: 1.41x faster                                              |
| docutils       | 3.30 sec                                               | 2.64 sec: 1.25x faster                                             |
| tornado_http   | 136 ms                                                 | 94.8 ms: 1.44x faster                                              |
| Geometric mean | (ref)                                                  | 1.35x faster                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 433 ms: 1.68x faster                                               |
| async_tree_memoization  | 870 ms                                                 | 561 ms: 1.55x faster                                               |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.50x faster                                             |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 705 ms: 1.44x faster                                               |
| Geometric mean          | (ref)                                                  | 1.54x faster                                                       |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 88.6 ms: 1.73x faster                                              |
| float          | 117 ms                                                 | 80.5 ms: 1.45x faster                                              |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                               |
| Geometric mean | (ref)                                                  | 1.37x faster                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 129 ms: 1.46x faster                                               |
| regex_v8       | 27.8 ms                                                | 25.4 ms: 1.09x faster                                              |
| regex_dna      | 227 ms                                                 | 221 ms: 1.02x faster                                               |
| regex_effbot   | 3.63 ms                                                | 3.55 ms: 1.02x faster                                              |
| Geometric mean | (ref)                                                  | 1.14x faster                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 299 us: 1.62x faster                                               |
| unpickle_pure_python | 331 us                                                 | 215 us: 1.54x faster                                               |
| tomli_loads          | 3.14 sec                                               | 2.14 sec: 1.47x faster                                             |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                              |
| xml_etree_process    | 79.1 ms                                                | 58.8 ms: 1.34x faster                                              |
| xml_etree_generate   | 99.4 ms                                                | 86.3 ms: 1.15x faster                                              |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                              |
| xml_etree_iterparse  | 115 ms                                                 | 105 ms: 1.10x faster                                               |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                               |
| pickle_list          | 5.08 us                                                | 5.11 us: 1.01x slower                                              |
| unpickle_list        | 5.20 us                                                | 5.32 us: 1.02x slower                                              |
| unpickle             | 14.4 us                                                | 14.9 us: 1.03x slower                                              |
| pickle               | 10.7 us                                                | 11.6 us: 1.09x slower                                              |
| pickle_dict          | 29.6 us                                                | 34.0 us: 1.15x slower                                              |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                       |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                              |
| python_startup_no_site | 5.93 ms                                                | 8.73 ms: 1.47x slower                                              |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.0 ms: 1.48x faster                                              |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 109 us: 4.99x faster                                               |
| generators               | 80.1 ms                                                | 29.4 ms: 2.72x faster                                              |
| deltablue                | 7.91 ms                                                | 3.22 ms: 2.46x faster                                              |
| chaos                    | 115 ms                                                 | 58.7 ms: 1.97x faster                                              |
| raytrace                 | 507 ms                                                 | 260 ms: 1.95x faster                                               |
| asyncio_tcp              | 922 ms                                                 | 482 ms: 1.91x faster                                               |
| logging_silent           | 190 ns                                                 | 103 ns: 1.84x faster                                               |
| scimark_sor              | 220 ms                                                 | 121 ms: 1.82x faster                                               |
| crypto_pyaes             | 128 ms                                                 | 71.7 ms: 1.78x faster                                              |
| richards_super           | 94.7 ms                                                | 53.2 ms: 1.78x faster                                              |
| comprehensions           | 28.8 us                                                | 16.2 us: 1.78x faster                                              |
| scimark_monte_carlo      | 118 ms                                                 | 66.6 ms: 1.78x faster                                              |
| go                       | 240 ms                                                 | 137 ms: 1.76x faster                                               |
| sqlglot_parse            | 2.17 ms                                                | 1.25 ms: 1.74x faster                                              |
| nbody                    | 154 ms                                                 | 88.6 ms: 1.73x faster                                              |
| hexiom                   | 10.4 ms                                                | 6.13 ms: 1.69x faster                                              |
| async_tree_none          | 728 ms                                                 | 433 ms: 1.68x faster                                               |
| richards                 | 79.3 ms                                                | 47.4 ms: 1.67x faster                                              |
| sqlglot_transpile        | 2.57 ms                                                | 1.58 ms: 1.63x faster                                              |
| pickle_pure_python       | 484 us                                                 | 299 us: 1.62x faster                                               |
| coroutines               | 35.1 ms                                                | 21.9 ms: 1.60x faster                                              |
| deepcopy_memo            | 58.5 us                                                | 37.3 us: 1.57x faster                                              |
| scimark_lu               | 176 ms                                                 | 113 ms: 1.56x faster                                               |
| pyflate                  | 716 ms                                                 | 458 ms: 1.56x faster                                               |
| async_tree_memoization   | 870 ms                                                 | 561 ms: 1.55x faster                                               |
| spectral_norm            | 170 ms                                                 | 110 ms: 1.55x faster                                               |
| unpickle_pure_python     | 331 us                                                 | 215 us: 1.54x faster                                               |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.50x faster                                             |
| mako                     | 16.3 ms                                                | 11.0 ms: 1.48x faster                                              |
| tomli_loads              | 3.14 sec                                               | 2.14 sec: 1.47x faster                                             |
| regex_compile            | 188 ms                                                 | 129 ms: 1.46x faster                                               |
| logging_simple           | 8.30 us                                                | 5.69 us: 1.46x faster                                              |
| float                    | 117 ms                                                 | 80.5 ms: 1.45x faster                                              |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.44x faster                                             |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                              |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 705 ms: 1.44x faster                                               |
| tornado_http             | 136 ms                                                 | 94.8 ms: 1.44x faster                                              |
| logging_format           | 9.09 us                                                | 6.33 us: 1.44x faster                                              |
| deepcopy                 | 479 us                                                 | 339 us: 1.41x faster                                               |
| chameleon                | 9.68 ms                                                | 6.87 ms: 1.41x faster                                              |
| pprint_pformat           | 2.10 sec                                               | 1.49 sec: 1.41x faster                                             |
| deepcopy_reduce          | 4.17 us                                                | 2.99 us: 1.39x faster                                              |
| pprint_safe_repr         | 1.02 sec                                               | 733 ms: 1.39x faster                                               |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.69 ms: 1.38x faster                                              |
| pycparser                | 1.58 sec                                               | 1.16 sec: 1.36x faster                                             |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                              |
| xml_etree_process        | 79.1 ms                                                | 58.8 ms: 1.34x faster                                              |
| sqlglot_normalize        | 143 ms                                                 | 107 ms: 1.34x faster                                               |
| nqueens                  | 106 ms                                                 | 79.4 ms: 1.33x faster                                              |
| 2to3                     | 348 ms                                                 | 263 ms: 1.33x faster                                               |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.32x faster                                              |
| sympy_sum                | 196 ms                                                 | 149 ms: 1.32x faster                                               |
| fannkuch                 | 532 ms                                                 | 402 ms: 1.32x faster                                               |
| scimark_fft              | 466 ms                                                 | 360 ms: 1.29x faster                                               |
| sqlglot_optimize         | 69.2 ms                                                | 53.9 ms: 1.28x faster                                              |
| dulwich_log              | 84.3 ms                                                | 65.9 ms: 1.28x faster                                              |
| sympy_str                | 346 ms                                                 | 273 ms: 1.27x faster                                               |
| docutils                 | 3.30 sec                                               | 2.64 sec: 1.25x faster                                             |
| sympy_expand             | 566 ms                                                 | 460 ms: 1.23x faster                                               |
| dask                     | 441 ms                                                 | 361 ms: 1.22x faster                                               |
| bench_thread_pool        | 986 us                                                 | 835 us: 1.18x faster                                               |
| xml_etree_generate       | 99.4 ms                                                | 86.3 ms: 1.15x faster                                              |
| mdp                      | 2.85 sec                                               | 2.53 sec: 1.13x faster                                             |
| pathlib                  | 20.5 ms                                                | 18.3 ms: 1.12x faster                                              |
| json_loads               | 31.2 us                                                | 28.1 us: 1.11x faster                                              |
| json                     | 5.69 ms                                                | 5.14 ms: 1.11x faster                                              |
| xml_etree_iterparse      | 115 ms                                                 | 105 ms: 1.10x faster                                               |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                              |
| meteor_contest           | 120 ms                                                 | 109 ms: 1.10x faster                                               |
| regex_v8                 | 27.8 ms                                                | 25.4 ms: 1.09x faster                                              |
| unpack_sequence          | 60.0 ns                                                | 55.0 ns: 1.09x faster                                              |
| sqlite_synth             | 3.02 us                                                | 2.82 us: 1.07x faster                                              |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.06x faster                                               |
| regex_dna                | 227 ms                                                 | 221 ms: 1.02x faster                                               |
| regex_effbot             | 3.63 ms                                                | 3.55 ms: 1.02x faster                                              |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                               |
| async_generators         | 444 ms                                                 | 441 ms: 1.01x faster                                               |
| asyncio_websockets       | 559 ms                                                 | 556 ms: 1.00x faster                                               |
| pickle_list              | 5.08 us                                                | 5.11 us: 1.01x slower                                              |
| unpickle_list            | 5.20 us                                                | 5.32 us: 1.02x slower                                              |
| gc_traversal             | 3.62 ms                                                | 3.74 ms: 1.03x slower                                              |
| unpickle                 | 14.4 us                                                | 14.9 us: 1.03x slower                                              |
| pickle                   | 10.7 us                                                | 11.6 us: 1.09x slower                                              |
| telco                    | 7.27 ms                                                | 8.33 ms: 1.15x slower                                              |
| pickle_dict              | 29.6 us                                                | 34.0 us: 1.15x slower                                              |
| coverage                 | 79.4 ms                                                | 93.9 ms: 1.18x slower                                              |
| python_startup_no_site   | 5.93 ms                                                | 8.73 ms: 1.47x slower                                              |
| Geometric mean           | (ref)                                                  | 1.36x faster                                                       |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240123-3.13.0a3+-f5a8425/bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.32x
- 95% likely to have a speedup of 1.31x
- 99% likely to have a speedup of 1.29x


# Memory

- memory change: 1.05x