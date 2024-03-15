# Results vs. 3.10.4

- fork: mdboom
- ref: too_short_7
- machine: linux-x86_64
- commit hash: 61ce027
- commit date: 2024-03-13
- overall geometric mean: 1.30x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.33x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 281 ms: 1.24x faster                                          |
| chameleon      | 9.68 ms                                                | 7.01 ms: 1.38x faster                                         |
| docutils       | 3.30 sec                                               | 2.78 sec: 1.19x faster                                        |
| html5lib       | 88.9 ms                                                | 68.1 ms: 1.30x faster                                         |
| tornado_http   | 136 ms                                                 | 98.8 ms: 1.38x faster                                         |
| Geometric mean | (ref)                                                  | 1.30x faster                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 446 ms: 1.63x faster                                          |
| async_tree_memoization  | 870 ms                                                 | 576 ms: 1.51x faster                                          |
| async_tree_io           | 1.77 sec                                               | 1.21 sec: 1.46x faster                                        |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 727 ms: 1.40x faster                                          |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 93.5 ms: 1.64x faster                                         |
| float          | 117 ms                                                 | 80.6 ms: 1.45x faster                                         |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                          |
| Geometric mean | (ref)                                                  | 1.34x faster                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 143 ms: 1.32x faster                                          |
| regex_v8       | 27.8 ms                                                | 26.1 ms: 1.07x faster                                         |
| regex_dna      | 227 ms                                                 | 232 ms: 1.02x slower                                          |
| regex_effbot   | 3.63 ms                                                | 3.83 ms: 1.06x slower                                         |
| Geometric mean | (ref)                                                  | 1.07x faster                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 298 us: 1.62x faster                                          |
| tomli_loads          | 3.14 sec                                               | 2.07 sec: 1.52x faster                                        |
| unpickle_pure_python | 331 us                                                 | 238 us: 1.39x faster                                          |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                         |
| xml_etree_process    | 79.1 ms                                                | 59.7 ms: 1.32x faster                                         |
| xml_etree_generate   | 99.4 ms                                                | 87.4 ms: 1.14x faster                                         |
| json_loads           | 31.2 us                                                | 28.0 us: 1.11x faster                                         |
| xml_etree_iterparse  | 115 ms                                                 | 107 ms: 1.08x faster                                          |
| unpickle_list        | 5.20 us                                                | 4.89 us: 1.06x faster                                         |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                          |
| pickle_list          | 5.08 us                                                | 4.95 us: 1.03x faster                                         |
| unpickle             | 14.4 us                                                | 14.8 us: 1.03x slower                                         |
| pickle               | 10.7 us                                                | 11.6 us: 1.09x slower                                         |
| pickle_dict          | 29.6 us                                                | 33.7 us: 1.14x slower                                         |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 12.6 ms: 1.16x faster                                         |
| python_startup_no_site | 5.93 ms                                                | 11.1 ms: 1.88x slower                                         |
| Geometric mean         | (ref)                                                  | 1.27x slower                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 10.9 ms: 1.50x faster                                         |
| django_template | 48.2 ms                                                | 34.8 ms: 1.39x faster                                         |
| genshi_text     | 31.8 ms                                                | 24.0 ms: 1.33x faster                                         |
| genshi_xml      | 66.0 ms                                                | 55.0 ms: 1.20x faster                                         |
| Geometric mean  | (ref)                                                  | 1.35x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|--------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 111 us: 4.91x faster                                          |
| generators               | 80.1 ms                                                | 29.6 ms: 2.71x faster                                         |
| deltablue                | 7.91 ms                                                | 3.43 ms: 2.30x faster                                         |
| logging_silent           | 190 ns                                                 | 101 ns: 1.88x faster                                          |
| asyncio_tcp              | 922 ms                                                 | 504 ms: 1.83x faster                                          |
| richards_super           | 94.7 ms                                                | 52.5 ms: 1.80x faster                                         |
| chaos                    | 115 ms                                                 | 64.5 ms: 1.79x faster                                         |
| raytrace                 | 507 ms                                                 | 291 ms: 1.74x faster                                          |
| scimark_sor              | 220 ms                                                 | 128 ms: 1.71x faster                                          |
| richards                 | 79.3 ms                                                | 46.5 ms: 1.71x faster                                         |
| pylint                   | 551 ms                                                 | 324 ms: 1.70x faster                                          |
| crypto_pyaes             | 128 ms                                                 | 75.8 ms: 1.69x faster                                         |
| scimark_monte_carlo      | 118 ms                                                 | 71.0 ms: 1.67x faster                                         |
| comprehensions           | 28.8 us                                                | 17.3 us: 1.66x faster                                         |
| sqlglot_parse            | 2.17 ms                                                | 1.32 ms: 1.65x faster                                         |
| nbody                    | 154 ms                                                 | 93.5 ms: 1.64x faster                                         |
| async_tree_none          | 728 ms                                                 | 446 ms: 1.63x faster                                          |
| pickle_pure_python       | 484 us                                                 | 298 us: 1.62x faster                                          |
| go                       | 240 ms                                                 | 149 ms: 1.61x faster                                          |
| coroutines               | 35.1 ms                                                | 22.4 ms: 1.56x faster                                         |
| sqlglot_transpile        | 2.57 ms                                                | 1.66 ms: 1.55x faster                                         |
| tomli_loads              | 3.14 sec                                               | 2.07 sec: 1.52x faster                                        |
| async_tree_memoization   | 870 ms                                                 | 576 ms: 1.51x faster                                          |
| mako                     | 16.3 ms                                                | 10.9 ms: 1.50x faster                                         |
| pyflate                  | 716 ms                                                 | 482 ms: 1.49x faster                                          |
| spectral_norm            | 170 ms                                                 | 115 ms: 1.48x faster                                          |
| hexiom                   | 10.4 ms                                                | 7.04 ms: 1.48x faster                                         |
| deepcopy_memo            | 58.5 us                                                | 39.7 us: 1.47x faster                                         |
| async_tree_io            | 1.77 sec                                               | 1.21 sec: 1.46x faster                                        |
| float                    | 117 ms                                                 | 80.6 ms: 1.45x faster                                         |
| logging_simple           | 8.30 us                                                | 5.92 us: 1.40x faster                                         |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 727 ms: 1.40x faster                                          |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.85 sec: 1.39x faster                                        |
| unpickle_pure_python     | 331 us                                                 | 238 us: 1.39x faster                                          |
| logging_format           | 9.09 us                                                | 6.56 us: 1.39x faster                                         |
| django_template          | 48.2 ms                                                | 34.8 ms: 1.39x faster                                         |
| chameleon                | 9.68 ms                                                | 7.01 ms: 1.38x faster                                         |
| tornado_http             | 136 ms                                                 | 98.8 ms: 1.38x faster                                         |
| scimark_lu               | 176 ms                                                 | 129 ms: 1.37x faster                                          |
| pprint_pformat           | 2.10 sec                                               | 1.56 sec: 1.35x faster                                        |
| fannkuch                 | 532 ms                                                 | 394 ms: 1.35x faster                                          |
| pprint_safe_repr         | 1.02 sec                                               | 755 ms: 1.35x faster                                          |
| thrift                   | 1.07 ms                                                | 794 us: 1.35x faster                                          |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                         |
| scimark_fft              | 466 ms                                                 | 345 ms: 1.35x faster                                          |
| deepcopy                 | 479 us                                                 | 356 us: 1.35x faster                                          |
| deepcopy_reduce          | 4.17 us                                                | 3.11 us: 1.34x faster                                         |
| genshi_text              | 31.8 ms                                                | 24.0 ms: 1.33x faster                                         |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.88 ms: 1.33x faster                                         |
| xml_etree_process        | 79.1 ms                                                | 59.7 ms: 1.32x faster                                         |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.32x faster                                          |
| regex_compile            | 188 ms                                                 | 143 ms: 1.32x faster                                          |
| html5lib                 | 88.9 ms                                                | 68.1 ms: 1.30x faster                                         |
| pycparser                | 1.58 sec                                               | 1.27 sec: 1.24x faster                                        |
| 2to3                     | 348 ms                                                 | 281 ms: 1.24x faster                                          |
| sqlglot_optimize         | 69.2 ms                                                | 56.4 ms: 1.23x faster                                         |
| sympy_integrate          | 25.8 ms                                                | 21.2 ms: 1.22x faster                                         |
| sympy_sum                | 196 ms                                                 | 162 ms: 1.21x faster                                          |
| dulwich_log              | 84.3 ms                                                | 69.7 ms: 1.21x faster                                         |
| sympy_str                | 346 ms                                                 | 287 ms: 1.20x faster                                          |
| genshi_xml               | 66.0 ms                                                | 55.0 ms: 1.20x faster                                         |
| aiohttp                  | 1.44 ms                                                | 1.20 ms: 1.20x faster                                         |
| docutils                 | 3.30 sec                                               | 2.78 sec: 1.19x faster                                        |
| djangocms                | 38.4 us                                                | 32.4 us: 1.19x faster                                         |
| dask                     | 441 ms                                                 | 374 ms: 1.18x faster                                          |
| gunicorn                 | 1.53 ms                                                | 1.30 ms: 1.18x faster                                         |
| nqueens                  | 106 ms                                                 | 90.0 ms: 1.18x faster                                         |
| sympy_expand             | 566 ms                                                 | 485 ms: 1.17x faster                                          |
| python_startup           | 14.6 ms                                                | 12.6 ms: 1.16x faster                                         |
| bench_thread_pool        | 986 us                                                 | 863 us: 1.14x faster                                          |
| xml_etree_generate       | 99.4 ms                                                | 87.4 ms: 1.14x faster                                         |
| json_loads               | 31.2 us                                                | 28.0 us: 1.11x faster                                         |
| json                     | 5.69 ms                                                | 5.12 ms: 1.11x faster                                         |
| meteor_contest           | 120 ms                                                 | 109 ms: 1.10x faster                                          |
| pathlib                  | 20.5 ms                                                | 18.8 ms: 1.09x faster                                         |
| mdp                      | 2.85 sec                                               | 2.63 sec: 1.08x faster                                        |
| xml_etree_iterparse      | 115 ms                                                 | 107 ms: 1.08x faster                                          |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                         |
| regex_v8                 | 27.8 ms                                                | 26.1 ms: 1.07x faster                                         |
| unpickle_list            | 5.20 us                                                | 4.89 us: 1.06x faster                                         |
| sqlite_synth             | 3.02 us                                                | 2.85 us: 1.06x faster                                         |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.06x faster                                          |
| pickle_list              | 5.08 us                                                | 4.95 us: 1.03x faster                                         |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                          |
| asyncio_websockets       | 559 ms                                                 | 563 ms: 1.01x slower                                          |
| gc_traversal             | 3.62 ms                                                | 3.69 ms: 1.02x slower                                         |
| async_generators         | 444 ms                                                 | 453 ms: 1.02x slower                                          |
| regex_dna                | 227 ms                                                 | 232 ms: 1.02x slower                                          |
| unpickle                 | 14.4 us                                                | 14.8 us: 1.03x slower                                         |
| regex_effbot             | 3.63 ms                                                | 3.83 ms: 1.06x slower                                         |
| pickle                   | 10.7 us                                                | 11.6 us: 1.09x slower                                         |
| bench_mp_pool            | 24.0 ms                                                | 26.3 ms: 1.09x slower                                         |
| pickle_dict              | 29.6 us                                                | 33.7 us: 1.14x slower                                         |
| telco                    | 7.27 ms                                                | 8.56 ms: 1.18x slower                                         |
| coverage                 | 79.4 ms                                                | 98.0 ms: 1.23x slower                                         |
| unpack_sequence          | 60.0 ns                                                | 87.8 ns: 1.46x slower                                         |
| python_startup_no_site   | 5.93 ms                                                | 11.1 ms: 1.88x slower                                         |
| Geometric mean           | (ref)                                                  | 1.30x faster                                                  |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240313-3.13.0a5+-61ce027-JIT/bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.24x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.33x