
# Results vs. 3.10.4

- fork: mdboom
- ref: rare_event_stats
- machine: linux-x86_64
- commit hash: 937bd66
- commit date: 2024-01-22
- overall geometric mean: 1.36x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.29x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 264 ms: 1.32x faster                                               |
| chameleon      | 9.68 ms                                                | 7.06 ms: 1.37x faster                                              |
| docutils       | 3.30 sec                                               | 2.60 sec: 1.27x faster                                             |
| tornado_http   | 136 ms                                                 | 94.2 ms: 1.45x faster                                              |
| Geometric mean | (ref)                                                  | 1.35x faster                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 431 ms: 1.69x faster                                               |
| async_tree_memoization  | 870 ms                                                 | 560 ms: 1.55x faster                                               |
| async_tree_io           | 1.77 sec                                               | 1.17 sec: 1.51x faster                                             |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 702 ms: 1.45x faster                                               |
| Geometric mean          | (ref)                                                  | 1.55x faster                                                       |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 86.1 ms: 1.78x faster                                              |
| float          | 117 ms                                                 | 80.1 ms: 1.46x faster                                              |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                               |
| Geometric mean | (ref)                                                  | 1.38x faster                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 130 ms: 1.45x faster                                               |
| regex_v8       | 27.8 ms                                                | 25.5 ms: 1.09x faster                                              |
| regex_effbot   | 3.63 ms                                                | 3.54 ms: 1.03x faster                                              |
| regex_dna      | 227 ms                                                 | 222 ms: 1.02x faster                                               |
| Geometric mean | (ref)                                                  | 1.13x faster                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 297 us: 1.63x faster                                               |
| unpickle_pure_python | 331 us                                                 | 212 us: 1.56x faster                                               |
| tomli_loads          | 3.14 sec                                               | 2.12 sec: 1.48x faster                                             |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                              |
| xml_etree_process    | 79.1 ms                                                | 58.6 ms: 1.35x faster                                              |
| xml_etree_generate   | 99.4 ms                                                | 85.6 ms: 1.16x faster                                              |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                              |
| xml_etree_iterparse  | 115 ms                                                 | 104 ms: 1.11x faster                                               |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                               |
| pickle_list          | 5.08 us                                                | 5.27 us: 1.04x slower                                              |
| unpickle_list        | 5.20 us                                                | 5.41 us: 1.04x slower                                              |
| unpickle             | 14.4 us                                                | 15.4 us: 1.07x slower                                              |
| pickle               | 10.7 us                                                | 11.7 us: 1.10x slower                                              |
| pickle_dict          | 29.6 us                                                | 34.8 us: 1.18x slower                                              |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                       |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.45x faster                                              |
| python_startup_no_site | 5.93 ms                                                | 8.68 ms: 1.46x slower                                              |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.1 ms: 1.48x faster                                              |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.93x faster                                               |
| generators               | 80.1 ms                                                | 29.3 ms: 2.73x faster                                              |
| deltablue                | 7.91 ms                                                | 3.15 ms: 2.51x faster                                              |
| raytrace                 | 507 ms                                                 | 257 ms: 1.97x faster                                               |
| chaos                    | 115 ms                                                 | 59.5 ms: 1.94x faster                                              |
| asyncio_tcp              | 922 ms                                                 | 480 ms: 1.92x faster                                               |
| scimark_sor              | 220 ms                                                 | 121 ms: 1.81x faster                                               |
| crypto_pyaes             | 128 ms                                                 | 70.9 ms: 1.80x faster                                              |
| logging_silent           | 190 ns                                                 | 106 ns: 1.79x faster                                               |
| comprehensions           | 28.8 us                                                | 16.1 us: 1.79x faster                                              |
| nbody                    | 154 ms                                                 | 86.1 ms: 1.78x faster                                              |
| scimark_monte_carlo      | 118 ms                                                 | 66.4 ms: 1.78x faster                                              |
| richards_super           | 94.7 ms                                                | 53.3 ms: 1.78x faster                                              |
| hexiom                   | 10.4 ms                                                | 5.89 ms: 1.76x faster                                              |
| go                       | 240 ms                                                 | 137 ms: 1.76x faster                                               |
| sqlglot_parse            | 2.17 ms                                                | 1.25 ms: 1.73x faster                                              |
| async_tree_none          | 728 ms                                                 | 431 ms: 1.69x faster                                               |
| richards                 | 79.3 ms                                                | 47.4 ms: 1.67x faster                                              |
| sqlglot_transpile        | 2.57 ms                                                | 1.58 ms: 1.63x faster                                              |
| pickle_pure_python       | 484 us                                                 | 297 us: 1.63x faster                                               |
| spectral_norm            | 170 ms                                                 | 108 ms: 1.57x faster                                               |
| coroutines               | 35.1 ms                                                | 22.3 ms: 1.57x faster                                              |
| scimark_lu               | 176 ms                                                 | 113 ms: 1.56x faster                                               |
| unpickle_pure_python     | 331 us                                                 | 212 us: 1.56x faster                                               |
| pyflate                  | 716 ms                                                 | 460 ms: 1.56x faster                                               |
| async_tree_memoization   | 870 ms                                                 | 560 ms: 1.55x faster                                               |
| deepcopy_memo            | 58.5 us                                                | 37.7 us: 1.55x faster                                              |
| async_tree_io            | 1.77 sec                                               | 1.17 sec: 1.51x faster                                             |
| tomli_loads              | 3.14 sec                                               | 2.12 sec: 1.48x faster                                             |
| mako                     | 16.3 ms                                                | 11.1 ms: 1.48x faster                                              |
| float                    | 117 ms                                                 | 80.1 ms: 1.46x faster                                              |
| regex_compile            | 188 ms                                                 | 130 ms: 1.45x faster                                               |
| logging_format           | 9.09 us                                                | 6.26 us: 1.45x faster                                              |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.45x faster                                              |
| tornado_http             | 136 ms                                                 | 94.2 ms: 1.45x faster                                              |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 702 ms: 1.45x faster                                               |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.44x faster                                             |
| logging_simple           | 8.30 us                                                | 5.76 us: 1.44x faster                                              |
| pprint_pformat           | 2.10 sec                                               | 1.51 sec: 1.40x faster                                             |
| pprint_safe_repr         | 1.02 sec                                               | 736 ms: 1.38x faster                                               |
| deepcopy                 | 479 us                                                 | 348 us: 1.38x faster                                               |
| chameleon                | 9.68 ms                                                | 7.06 ms: 1.37x faster                                              |
| pycparser                | 1.58 sec                                               | 1.15 sec: 1.37x faster                                             |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                              |
| deepcopy_reduce          | 4.17 us                                                | 3.07 us: 1.36x faster                                              |
| xml_etree_process        | 79.1 ms                                                | 58.6 ms: 1.35x faster                                              |
| sqlglot_normalize        | 143 ms                                                 | 107 ms: 1.33x faster                                               |
| scimark_fft              | 466 ms                                                 | 350 ms: 1.33x faster                                               |
| unpack_sequence          | 60.0 ns                                                | 45.2 ns: 1.33x faster                                              |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.32x faster                                              |
| 2to3                     | 348 ms                                                 | 264 ms: 1.32x faster                                               |
| sympy_sum                | 196 ms                                                 | 149 ms: 1.32x faster                                               |
| nqueens                  | 106 ms                                                 | 80.1 ms: 1.32x faster                                              |
| fannkuch                 | 532 ms                                                 | 403 ms: 1.32x faster                                               |
| dulwich_log              | 84.3 ms                                                | 65.3 ms: 1.29x faster                                              |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.05 ms: 1.28x faster                                              |
| sqlglot_optimize         | 69.2 ms                                                | 54.2 ms: 1.28x faster                                              |
| docutils                 | 3.30 sec                                               | 2.60 sec: 1.27x faster                                             |
| sympy_str                | 346 ms                                                 | 279 ms: 1.24x faster                                               |
| dask                     | 441 ms                                                 | 360 ms: 1.22x faster                                               |
| sympy_expand             | 566 ms                                                 | 464 ms: 1.22x faster                                               |
| bench_thread_pool        | 986 us                                                 | 825 us: 1.20x faster                                               |
| xml_etree_generate       | 99.4 ms                                                | 85.6 ms: 1.16x faster                                              |
| pathlib                  | 20.5 ms                                                | 18.3 ms: 1.12x faster                                              |
| json                     | 5.69 ms                                                | 5.11 ms: 1.11x faster                                              |
| json_loads               | 31.2 us                                                | 28.1 us: 1.11x faster                                              |
| xml_etree_iterparse      | 115 ms                                                 | 104 ms: 1.11x faster                                               |
| meteor_contest           | 120 ms                                                 | 108 ms: 1.11x faster                                               |
| create_gc_cycles         | 1.62 ms                                                | 1.46 ms: 1.11x faster                                              |
| regex_v8                 | 27.8 ms                                                | 25.5 ms: 1.09x faster                                              |
| sqlite_synth             | 3.02 us                                                | 2.81 us: 1.08x faster                                              |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                               |
| mdp                      | 2.85 sec                                               | 2.73 sec: 1.04x faster                                             |
| regex_effbot             | 3.63 ms                                                | 3.54 ms: 1.03x faster                                              |
| regex_dna                | 227 ms                                                 | 222 ms: 1.02x faster                                               |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                               |
| async_generators         | 444 ms                                                 | 442 ms: 1.00x faster                                               |
| pickle_list              | 5.08 us                                                | 5.27 us: 1.04x slower                                              |
| unpickle_list            | 5.20 us                                                | 5.41 us: 1.04x slower                                              |
| unpickle                 | 14.4 us                                                | 15.4 us: 1.07x slower                                              |
| gc_traversal             | 3.62 ms                                                | 3.94 ms: 1.09x slower                                              |
| pickle                   | 10.7 us                                                | 11.7 us: 1.10x slower                                              |
| telco                    | 7.27 ms                                                | 8.24 ms: 1.13x slower                                              |
| pickle_dict              | 29.6 us                                                | 34.8 us: 1.18x slower                                              |
| coverage                 | 79.4 ms                                                | 94.4 ms: 1.19x slower                                              |
| python_startup_no_site   | 5.93 ms                                                | 8.68 ms: 1.46x slower                                              |
| Geometric mean           | (ref)                                                  | 1.36x faster                                                       |

Benchmark hidden because not significant (3): mypy2, asyncio_websockets, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240122-3.13.0a3+-937bd66/bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.32x
- 95% likely to have a speedup of 1.31x
- 99% likely to have a speedup of 1.29x


# Memory

- memory change: 1.06x