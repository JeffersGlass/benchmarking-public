# Results vs. 3.10.4

- fork: jeffersglass
- ref: justin_supernodes_on
- machine: linux-x86_64
- commit hash: f486338
- commit date: 2024-03-16
- overall geometric mean: 1.32x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: 1.32x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 297 ms: 1.17x faster                                                         |
| chameleon      | 9.68 ms                                                | 7.25 ms: 1.34x faster                                                        |
| docutils       | 3.30 sec                                               | 2.67 sec: 1.24x faster                                                       |
| html5lib       | 88.9 ms                                                | 71.7 ms: 1.24x faster                                                        |
| tornado_http   | 136 ms                                                 | 147 ms: 1.08x slower                                                         |
| Geometric mean | (ref)                                                  | 1.17x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 449 ms: 1.62x faster                                                         |
| async_tree_io           | 1.77 sec                                               | 1.16 sec: 1.52x faster                                                       |
| async_tree_memoization  | 870 ms                                                 | 581 ms: 1.50x faster                                                         |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 698 ms: 1.46x faster                                                         |
| Geometric mean          | (ref)                                                  | 1.52x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 103 ms: 1.50x faster                                                         |
| float          | 117 ms                                                 | 78.5 ms: 1.49x faster                                                        |
| pidigits       | 191 ms                                                 | 188 ms: 1.01x faster                                                         |
| Geometric mean | (ref)                                                  | 1.31x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 136 ms: 1.39x faster                                                         |
| regex_dna      | 227 ms                                                 | 191 ms: 1.19x faster                                                         |
| regex_v8       | 27.8 ms                                                | 23.8 ms: 1.17x faster                                                        |
| regex_effbot   | 3.63 ms                                                | 3.37 ms: 1.08x faster                                                        |
| Geometric mean | (ref)                                                  | 1.20x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| tomli_loads          | 3.14 sec                                               | 1.93 sec: 1.63x faster                                                       |
| pickle_pure_python   | 484 us                                                 | 304 us: 1.59x faster                                                         |
| unpickle_pure_python | 331 us                                                 | 223 us: 1.49x faster                                                         |
| json_dumps           | 14.2 ms                                                | 9.56 ms: 1.48x faster                                                        |
| pickle_list          | 5.08 us                                                | 3.76 us: 1.35x faster                                                        |
| xml_etree_process    | 79.1 ms                                                | 59.9 ms: 1.32x faster                                                        |
| json_loads           | 31.2 us                                                | 23.9 us: 1.31x faster                                                        |
| unpickle_list        | 5.20 us                                                | 4.43 us: 1.17x faster                                                        |
| xml_etree_generate   | 99.4 ms                                                | 85.3 ms: 1.17x faster                                                        |
| xml_etree_iterparse  | 115 ms                                                 | 100 ms: 1.15x faster                                                         |
| xml_etree_parse      | 168 ms                                                 | 147 ms: 1.14x faster                                                         |
| pickle               | 10.7 us                                                | 9.75 us: 1.09x faster                                                        |
| pickle_dict          | 29.6 us                                                | 27.8 us: 1.06x faster                                                        |
| unpickle             | 14.4 us                                                | 13.5 us: 1.06x faster                                                        |
| Geometric mean       | (ref)                                                  | 1.27x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 19.2 ms: 1.31x slower                                                        |
| python_startup_no_site | 5.93 ms                                                | 17.8 ms: 3.00x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.98x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 9.85 ms: 1.66x faster                                                        |
| django_template | 48.2 ms                                                | 34.6 ms: 1.39x faster                                                        |
| genshi_text     | 31.8 ms                                                | 24.7 ms: 1.29x faster                                                        |
| genshi_xml      | 66.0 ms                                                | 54.2 ms: 1.22x faster                                                        |
| Geometric mean  | (ref)                                                  | 1.38x faster                                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 111 us: 4.92x faster                                                         |
| generators               | 80.1 ms                                                | 31.3 ms: 2.55x faster                                                        |
| deltablue                | 7.91 ms                                                | 3.75 ms: 2.11x faster                                                        |
| crypto_pyaes             | 128 ms                                                 | 65.4 ms: 1.95x faster                                                        |
| chaos                    | 115 ms                                                 | 61.3 ms: 1.88x faster                                                        |
| logging_silent           | 190 ns                                                 | 103 ns: 1.85x faster                                                         |
| spectral_norm            | 170 ms                                                 | 92.7 ms: 1.83x faster                                                        |
| raytrace                 | 507 ms                                                 | 287 ms: 1.77x faster                                                         |
| comprehensions           | 28.8 us                                                | 16.4 us: 1.75x faster                                                        |
| richards_super           | 94.7 ms                                                | 54.3 ms: 1.75x faster                                                        |
| pylint                   | 551 ms                                                 | 323 ms: 1.71x faster                                                         |
| scimark_monte_carlo      | 118 ms                                                 | 69.6 ms: 1.70x faster                                                        |
| richards                 | 79.3 ms                                                | 46.8 ms: 1.69x faster                                                        |
| sqlglot_parse            | 2.17 ms                                                | 1.30 ms: 1.66x faster                                                        |
| hexiom                   | 10.4 ms                                                | 6.26 ms: 1.66x faster                                                        |
| mako                     | 16.3 ms                                                | 9.85 ms: 1.66x faster                                                        |
| tomli_loads              | 3.14 sec                                               | 1.93 sec: 1.63x faster                                                       |
| async_tree_none          | 728 ms                                                 | 449 ms: 1.62x faster                                                         |
| deepcopy_memo            | 58.5 us                                                | 36.3 us: 1.61x faster                                                        |
| pickle_pure_python       | 484 us                                                 | 304 us: 1.59x faster                                                         |
| sqlglot_transpile        | 2.57 ms                                                | 1.65 ms: 1.56x faster                                                        |
| asyncio_tcp              | 922 ms                                                 | 592 ms: 1.56x faster                                                         |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.16 ms: 1.55x faster                                                        |
| fannkuch                 | 532 ms                                                 | 343 ms: 1.55x faster                                                         |
| scimark_fft              | 466 ms                                                 | 303 ms: 1.54x faster                                                         |
| async_tree_io            | 1.77 sec                                               | 1.16 sec: 1.52x faster                                                       |
| go                       | 240 ms                                                 | 159 ms: 1.51x faster                                                         |
| scimark_sor              | 220 ms                                                 | 146 ms: 1.50x faster                                                         |
| bench_mp_pool            | 24.0 ms                                                | 16.0 ms: 1.50x faster                                                        |
| async_tree_memoization   | 870 ms                                                 | 581 ms: 1.50x faster                                                         |
| nbody                    | 154 ms                                                 | 103 ms: 1.50x faster                                                         |
| float                    | 117 ms                                                 | 78.5 ms: 1.49x faster                                                        |
| scimark_lu               | 176 ms                                                 | 118 ms: 1.49x faster                                                         |
| unpickle_pure_python     | 331 us                                                 | 223 us: 1.49x faster                                                         |
| json_dumps               | 14.2 ms                                                | 9.56 ms: 1.48x faster                                                        |
| create_gc_cycles         | 1.62 ms                                                | 1.10 ms: 1.47x faster                                                        |
| pyflate                  | 716 ms                                                 | 489 ms: 1.46x faster                                                         |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.76 sec: 1.46x faster                                                       |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 698 ms: 1.46x faster                                                         |
| deepcopy                 | 479 us                                                 | 340 us: 1.41x faster                                                         |
| django_template          | 48.2 ms                                                | 34.6 ms: 1.39x faster                                                        |
| regex_compile            | 188 ms                                                 | 136 ms: 1.39x faster                                                         |
| thrift                   | 1.07 ms                                                | 774 us: 1.39x faster                                                         |
| coroutines               | 35.1 ms                                                | 25.4 ms: 1.38x faster                                                        |
| logging_format           | 9.09 us                                                | 6.64 us: 1.37x faster                                                        |
| logging_simple           | 8.30 us                                                | 6.09 us: 1.36x faster                                                        |
| pprint_pformat           | 2.10 sec                                               | 1.55 sec: 1.36x faster                                                       |
| pprint_safe_repr         | 1.02 sec                                               | 750 ms: 1.36x faster                                                         |
| pickle_list              | 5.08 us                                                | 3.76 us: 1.35x faster                                                        |
| chameleon                | 9.68 ms                                                | 7.25 ms: 1.34x faster                                                        |
| deepcopy_reduce          | 4.17 us                                                | 3.13 us: 1.33x faster                                                        |
| xml_etree_process        | 79.1 ms                                                | 59.9 ms: 1.32x faster                                                        |
| json_loads               | 31.2 us                                                | 23.9 us: 1.31x faster                                                        |
| sqlglot_normalize        | 143 ms                                                 | 109 ms: 1.31x faster                                                         |
| sympy_sum                | 196 ms                                                 | 152 ms: 1.29x faster                                                         |
| genshi_text              | 31.8 ms                                                | 24.7 ms: 1.29x faster                                                        |
| sympy_str                | 346 ms                                                 | 276 ms: 1.25x faster                                                         |
| json                     | 5.69 ms                                                | 4.58 ms: 1.24x faster                                                        |
| html5lib                 | 88.9 ms                                                | 71.7 ms: 1.24x faster                                                        |
| docutils                 | 3.30 sec                                               | 2.67 sec: 1.24x faster                                                       |
| sympy_integrate          | 25.8 ms                                                | 21.0 ms: 1.23x faster                                                        |
| nqueens                  | 106 ms                                                 | 86.3 ms: 1.23x faster                                                        |
| genshi_xml               | 66.0 ms                                                | 54.2 ms: 1.22x faster                                                        |
| sqlglot_optimize         | 69.2 ms                                                | 56.9 ms: 1.22x faster                                                        |
| sympy_expand             | 566 ms                                                 | 469 ms: 1.21x faster                                                         |
| pycparser                | 1.58 sec                                               | 1.31 sec: 1.20x faster                                                       |
| regex_dna                | 227 ms                                                 | 191 ms: 1.19x faster                                                         |
| meteor_contest           | 120 ms                                                 | 101 ms: 1.19x faster                                                         |
| 2to3                     | 348 ms                                                 | 297 ms: 1.17x faster                                                         |
| unpickle_list            | 5.20 us                                                | 4.43 us: 1.17x faster                                                        |
| xml_etree_generate       | 99.4 ms                                                | 85.3 ms: 1.17x faster                                                        |
| regex_v8                 | 27.8 ms                                                | 23.8 ms: 1.17x faster                                                        |
| xml_etree_iterparse      | 115 ms                                                 | 100 ms: 1.15x faster                                                         |
| xml_etree_parse          | 168 ms                                                 | 147 ms: 1.14x faster                                                         |
| sqlite_synth             | 3.02 us                                                | 2.69 us: 1.13x faster                                                        |
| mdp                      | 2.85 sec                                               | 2.54 sec: 1.12x faster                                                       |
| gc_traversal             | 3.62 ms                                                | 3.27 ms: 1.11x faster                                                        |
| async_generators         | 444 ms                                                 | 405 ms: 1.10x faster                                                         |
| pickle                   | 10.7 us                                                | 9.75 us: 1.09x faster                                                        |
| dulwich_log              | 84.3 ms                                                | 78.2 ms: 1.08x faster                                                        |
| regex_effbot             | 3.63 ms                                                | 3.37 ms: 1.08x faster                                                        |
| pickle_dict              | 29.6 us                                                | 27.8 us: 1.06x faster                                                        |
| unpickle                 | 14.4 us                                                | 13.5 us: 1.06x faster                                                        |
| pidigits                 | 191 ms                                                 | 188 ms: 1.01x faster                                                         |
| coverage                 | 79.4 ms                                                | 78.8 ms: 1.01x faster                                                        |
| telco                    | 7.27 ms                                                | 7.63 ms: 1.05x slower                                                        |
| tornado_http             | 136 ms                                                 | 147 ms: 1.08x slower                                                         |
| dask                     | 441 ms                                                 | 483 ms: 1.10x slower                                                         |
| pathlib                  | 20.5 ms                                                | 24.2 ms: 1.18x slower                                                        |
| asyncio_websockets       | 559 ms                                                 | 721 ms: 1.29x slower                                                         |
| python_startup           | 14.6 ms                                                | 19.2 ms: 1.31x slower                                                        |
| bench_thread_pool        | 986 us                                                 | 1.51 ms: 1.53x slower                                                        |
| unpack_sequence          | 60.0 ns                                                | 110 ns: 1.84x slower                                                         |
| python_startup_no_site   | 5.93 ms                                                | 17.8 ms: 3.00x slower                                                        |
| Geometric mean           | (ref)                                                  | 1.32x faster                                                                 |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, djangocms, flaskblogging, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240316-3.13.0a5+-f486338-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.28x
- 95% likely to have a speedup of 1.26x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: 1.32x