# Results vs. 3.10.4

- fork: jeffersglass
- ref: justin_supernodes_on
- machine: linux-x86_64
- commit hash: 54ce2b4
- commit date: 2024-03-16
- overall geometric mean: 1.42x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.35x faster
- Memory change: 1.31x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 273 ms: 1.28x faster                                                         |
| chameleon      | 9.68 ms                                                | 6.76 ms: 1.43x faster                                                        |
| docutils       | 3.30 sec                                               | 2.38 sec: 1.38x faster                                                       |
| html5lib       | 88.9 ms                                                | 67.5 ms: 1.32x faster                                                        |
| Geometric mean | (ref)                                                  | 1.27x faster                                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 389 ms: 1.87x faster                                                         |
| async_tree_memoization  | 870 ms                                                 | 494 ms: 1.76x faster                                                         |
| async_tree_io           | 1.77 sec                                               | 1.04 sec: 1.70x faster                                                       |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 611 ms: 1.66x faster                                                         |
| Geometric mean          | (ref)                                                  | 1.75x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 117 ms                                                 | 73.3 ms: 1.60x faster                                                        |
| nbody          | 154 ms                                                 | 99.6 ms: 1.54x faster                                                        |
| pidigits       | 191 ms                                                 | 174 ms: 1.09x faster                                                         |
| Geometric mean | (ref)                                                  | 1.39x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 125 ms: 1.50x faster                                                         |
| regex_dna      | 227 ms                                                 | 174 ms: 1.30x faster                                                         |
| regex_v8       | 27.8 ms                                                | 22.7 ms: 1.23x faster                                                        |
| regex_effbot   | 3.63 ms                                                | 3.07 ms: 1.18x faster                                                        |
| Geometric mean | (ref)                                                  | 1.30x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| tomli_loads          | 3.14 sec                                               | 1.85 sec: 1.70x faster                                                       |
| pickle_pure_python   | 484 us                                                 | 288 us: 1.68x faster                                                         |
| unpickle_pure_python | 331 us                                                 | 207 us: 1.60x faster                                                         |
| json_dumps           | 14.2 ms                                                | 8.95 ms: 1.58x faster                                                        |
| xml_etree_process    | 79.1 ms                                                | 55.3 ms: 1.43x faster                                                        |
| pickle_list          | 5.08 us                                                | 3.57 us: 1.42x faster                                                        |
| json_loads           | 31.2 us                                                | 22.4 us: 1.39x faster                                                        |
| xml_etree_iterparse  | 115 ms                                                 | 89.7 ms: 1.29x faster                                                        |
| xml_etree_generate   | 99.4 ms                                                | 79.0 ms: 1.26x faster                                                        |
| xml_etree_parse      | 168 ms                                                 | 134 ms: 1.25x faster                                                         |
| unpickle_list        | 5.20 us                                                | 4.22 us: 1.23x faster                                                        |
| pickle               | 10.7 us                                                | 8.98 us: 1.19x faster                                                        |
| unpickle             | 14.4 us                                                | 12.5 us: 1.15x faster                                                        |
| pickle_dict          | 29.6 us                                                | 26.2 us: 1.13x faster                                                        |
| Geometric mean       | (ref)                                                  | 1.37x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 17.2 ms: 1.18x slower                                                        |
| python_startup_no_site | 5.93 ms                                                | 15.9 ms: 2.67x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.78x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 9.10 ms: 1.79x faster                                                        |
| django_template | 48.2 ms                                                | 32.1 ms: 1.50x faster                                                        |
| genshi_text     | 31.8 ms                                                | 23.1 ms: 1.38x faster                                                        |
| genshi_xml      | 66.0 ms                                                | 50.1 ms: 1.32x faster                                                        |
| Geometric mean  | (ref)                                                  | 1.49x faster                                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 103 us: 5.27x faster                                                         |
| generators               | 80.1 ms                                                | 28.3 ms: 2.83x faster                                                        |
| deltablue                | 7.91 ms                                                | 3.51 ms: 2.25x faster                                                        |
| crypto_pyaes             | 128 ms                                                 | 61.9 ms: 2.07x faster                                                        |
| logging_silent           | 190 ns                                                 | 94.5 ns: 2.01x faster                                                        |
| chaos                    | 115 ms                                                 | 59.2 ms: 1.95x faster                                                        |
| pylint                   | 551 ms                                                 | 287 ms: 1.92x faster                                                         |
| spectral_norm            | 170 ms                                                 | 89.6 ms: 1.90x faster                                                        |
| comprehensions           | 28.8 us                                                | 15.3 us: 1.87x faster                                                        |
| async_tree_none          | 728 ms                                                 | 389 ms: 1.87x faster                                                         |
| raytrace                 | 507 ms                                                 | 273 ms: 1.85x faster                                                         |
| richards_super           | 94.7 ms                                                | 51.5 ms: 1.84x faster                                                        |
| mako                     | 16.3 ms                                                | 9.10 ms: 1.79x faster                                                        |
| asyncio_tcp              | 922 ms                                                 | 514 ms: 1.79x faster                                                         |
| richards                 | 79.3 ms                                                | 44.3 ms: 1.79x faster                                                        |
| scimark_monte_carlo      | 118 ms                                                 | 66.2 ms: 1.78x faster                                                        |
| deepcopy_memo            | 58.5 us                                                | 33.1 us: 1.77x faster                                                        |
| sqlglot_parse            | 2.17 ms                                                | 1.23 ms: 1.76x faster                                                        |
| async_tree_memoization   | 870 ms                                                 | 494 ms: 1.76x faster                                                         |
| hexiom                   | 10.4 ms                                                | 5.96 ms: 1.74x faster                                                        |
| sqlglot_transpile        | 2.57 ms                                                | 1.50 ms: 1.72x faster                                                        |
| async_tree_io            | 1.77 sec                                               | 1.04 sec: 1.70x faster                                                       |
| tomli_loads              | 3.14 sec                                               | 1.85 sec: 1.70x faster                                                       |
| pickle_pure_python       | 484 us                                                 | 288 us: 1.68x faster                                                         |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 3.89 ms: 1.66x faster                                                        |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 611 ms: 1.66x faster                                                         |
| fannkuch                 | 532 ms                                                 | 321 ms: 1.66x faster                                                         |
| bench_mp_pool            | 24.0 ms                                                | 14.5 ms: 1.66x faster                                                        |
| pyflate                  | 716 ms                                                 | 439 ms: 1.63x faster                                                         |
| go                       | 240 ms                                                 | 147 ms: 1.63x faster                                                         |
| scimark_lu               | 176 ms                                                 | 109 ms: 1.61x faster                                                         |
| scimark_fft              | 466 ms                                                 | 289 ms: 1.61x faster                                                         |
| unpickle_pure_python     | 331 us                                                 | 207 us: 1.60x faster                                                         |
| float                    | 117 ms                                                 | 73.3 ms: 1.60x faster                                                        |
| create_gc_cycles         | 1.62 ms                                                | 1.02 ms: 1.59x faster                                                        |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.61 sec: 1.59x faster                                                       |
| json_dumps               | 14.2 ms                                                | 8.95 ms: 1.58x faster                                                        |
| scimark_sor              | 220 ms                                                 | 140 ms: 1.57x faster                                                         |
| nbody                    | 154 ms                                                 | 99.6 ms: 1.54x faster                                                        |
| deepcopy                 | 479 us                                                 | 316 us: 1.51x faster                                                         |
| regex_compile            | 188 ms                                                 | 125 ms: 1.50x faster                                                         |
| django_template          | 48.2 ms                                                | 32.1 ms: 1.50x faster                                                        |
| thrift                   | 1.07 ms                                                | 717 us: 1.50x faster                                                         |
| coroutines               | 35.1 ms                                                | 23.7 ms: 1.48x faster                                                        |
| pprint_pformat           | 2.10 sec                                               | 1.43 sec: 1.47x faster                                                       |
| logging_simple           | 8.30 us                                                | 5.66 us: 1.47x faster                                                        |
| pprint_safe_repr         | 1.02 sec                                               | 697 ms: 1.46x faster                                                         |
| logging_format           | 9.09 us                                                | 6.25 us: 1.45x faster                                                        |
| chameleon                | 9.68 ms                                                | 6.76 ms: 1.43x faster                                                        |
| xml_etree_process        | 79.1 ms                                                | 55.3 ms: 1.43x faster                                                        |
| deepcopy_reduce          | 4.17 us                                                | 2.93 us: 1.43x faster                                                        |
| pickle_list              | 5.08 us                                                | 3.57 us: 1.42x faster                                                        |
| sympy_sum                | 196 ms                                                 | 139 ms: 1.42x faster                                                         |
| json_loads               | 31.2 us                                                | 22.4 us: 1.39x faster                                                        |
| docutils                 | 3.30 sec                                               | 2.38 sec: 1.38x faster                                                       |
| genshi_text              | 31.8 ms                                                | 23.1 ms: 1.38x faster                                                        |
| sympy_str                | 346 ms                                                 | 251 ms: 1.38x faster                                                         |
| pycparser                | 1.58 sec                                               | 1.16 sec: 1.35x faster                                                       |
| sympy_integrate          | 25.8 ms                                                | 19.1 ms: 1.35x faster                                                        |
| sqlglot_optimize         | 69.2 ms                                                | 51.7 ms: 1.34x faster                                                        |
| json                     | 5.69 ms                                                | 4.28 ms: 1.33x faster                                                        |
| sympy_expand             | 566 ms                                                 | 427 ms: 1.33x faster                                                         |
| genshi_xml               | 66.0 ms                                                | 50.1 ms: 1.32x faster                                                        |
| html5lib                 | 88.9 ms                                                | 67.5 ms: 1.32x faster                                                        |
| meteor_contest           | 120 ms                                                 | 91.5 ms: 1.31x faster                                                        |
| regex_dna                | 227 ms                                                 | 174 ms: 1.30x faster                                                         |
| nqueens                  | 106 ms                                                 | 81.4 ms: 1.30x faster                                                        |
| mdp                      | 2.85 sec                                               | 2.21 sec: 1.29x faster                                                       |
| xml_etree_iterparse      | 115 ms                                                 | 89.7 ms: 1.29x faster                                                        |
| 2to3                     | 348 ms                                                 | 273 ms: 1.28x faster                                                         |
| xml_etree_generate       | 99.4 ms                                                | 79.0 ms: 1.26x faster                                                        |
| xml_etree_parse          | 168 ms                                                 | 134 ms: 1.25x faster                                                         |
| unpickle_list            | 5.20 us                                                | 4.22 us: 1.23x faster                                                        |
| regex_v8                 | 27.8 ms                                                | 22.7 ms: 1.23x faster                                                        |
| gc_traversal             | 3.62 ms                                                | 2.97 ms: 1.22x faster                                                        |
| async_generators         | 444 ms                                                 | 364 ms: 1.22x faster                                                         |
| sqlite_synth             | 3.02 us                                                | 2.54 us: 1.19x faster                                                        |
| pickle                   | 10.7 us                                                | 8.98 us: 1.19x faster                                                        |
| regex_effbot             | 3.63 ms                                                | 3.07 ms: 1.18x faster                                                        |
| unpickle                 | 14.4 us                                                | 12.5 us: 1.15x faster                                                        |
| dulwich_log              | 84.3 ms                                                | 73.5 ms: 1.15x faster                                                        |
| mypy2                    | 894 ms                                                 | 788 ms: 1.13x faster                                                         |
| pickle_dict              | 29.6 us                                                | 26.2 us: 1.13x faster                                                        |
| pidigits                 | 191 ms                                                 | 174 ms: 1.09x faster                                                         |
| coverage                 | 79.4 ms                                                | 76.0 ms: 1.05x faster                                                        |
| telco                    | 7.27 ms                                                | 7.00 ms: 1.04x faster                                                        |
| pathlib                  | 20.5 ms                                                | 22.4 ms: 1.09x slower                                                        |
| python_startup           | 14.6 ms                                                | 17.2 ms: 1.18x slower                                                        |
| asyncio_websockets       | 559 ms                                                 | 669 ms: 1.20x slower                                                         |
| bench_thread_pool        | 986 us                                                 | 1.41 ms: 1.43x slower                                                        |
| unpack_sequence          | 60.0 ns                                                | 99.0 ns: 1.65x slower                                                        |
| sqlglot_normalize        | 143 ms                                                 | 269 ms: 1.88x slower                                                         |
| python_startup_no_site   | 5.93 ms                                                | 15.9 ms: 2.67x slower                                                        |
| Geometric mean           | (ref)                                                  | 1.42x faster                                                                 |

Benchmark hidden because not significant (2): dask, tornado_http
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, djangocms, flaskblogging, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240316-3.13.0a5+-54ce2b4-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.38x
- 95% likely to have a speedup of 1.37x
- 99% likely to have a speedup of 1.35x


# Memory

- memory change: 1.31x