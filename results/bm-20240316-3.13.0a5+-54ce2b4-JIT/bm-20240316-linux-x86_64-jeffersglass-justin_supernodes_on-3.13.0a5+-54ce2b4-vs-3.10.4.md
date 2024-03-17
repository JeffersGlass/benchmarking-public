# Results vs. 3.10.4

- fork: jeffersglass
- ref: justin_supernodes_on
- machine: linux-x86_64
- commit hash: 54ce2b4
- commit date: 2024-03-16
- overall geometric mean: 1.31x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: 1.31x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 304 ms: 1.15x faster                                                         |
| chameleon      | 9.68 ms                                                | 7.35 ms: 1.32x faster                                                        |
| docutils       | 3.30 sec                                               | 2.76 sec: 1.19x faster                                                       |
| html5lib       | 88.9 ms                                                | 73.5 ms: 1.21x faster                                                        |
| tornado_http   | 136 ms                                                 | 145 ms: 1.06x slower                                                         |
| Geometric mean | (ref)                                                  | 1.15x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 476 ms: 1.53x faster                                                         |
| async_tree_io           | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                       |
| async_tree_memoization  | 870 ms                                                 | 607 ms: 1.43x faster                                                         |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 728 ms: 1.40x faster                                                         |
| Geometric mean          | (ref)                                                  | 1.45x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 117 ms                                                 | 79.8 ms: 1.47x faster                                                        |
| nbody          | 154 ms                                                 | 107 ms: 1.44x faster                                                         |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                  | 1.29x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 134 ms: 1.41x faster                                                         |
| regex_dna      | 227 ms                                                 | 188 ms: 1.20x faster                                                         |
| regex_v8       | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                        |
| regex_effbot   | 3.63 ms                                                | 3.42 ms: 1.06x faster                                                        |
| Geometric mean | (ref)                                                  | 1.19x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| tomli_loads          | 3.14 sec                                               | 1.98 sec: 1.59x faster                                                       |
| pickle_pure_python   | 484 us                                                 | 308 us: 1.57x faster                                                         |
| json_dumps           | 14.2 ms                                                | 9.57 ms: 1.48x faster                                                        |
| unpickle_pure_python | 331 us                                                 | 223 us: 1.48x faster                                                         |
| xml_etree_process    | 79.1 ms                                                | 59.3 ms: 1.33x faster                                                        |
| pickle_list          | 5.08 us                                                | 3.83 us: 1.33x faster                                                        |
| json_loads           | 31.2 us                                                | 24.0 us: 1.30x faster                                                        |
| xml_etree_generate   | 99.4 ms                                                | 85.2 ms: 1.17x faster                                                        |
| xml_etree_iterparse  | 115 ms                                                 | 101 ms: 1.14x faster                                                         |
| unpickle_list        | 5.20 us                                                | 4.56 us: 1.14x faster                                                        |
| xml_etree_parse      | 168 ms                                                 | 148 ms: 1.13x faster                                                         |
| pickle               | 10.7 us                                                | 9.82 us: 1.09x faster                                                        |
| unpickle             | 14.4 us                                                | 13.7 us: 1.05x faster                                                        |
| pickle_dict          | 29.6 us                                                | 28.7 us: 1.03x faster                                                        |
| Geometric mean       | (ref)                                                  | 1.26x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 19.3 ms: 1.32x slower                                                        |
| python_startup_no_site | 5.93 ms                                                | 17.8 ms: 3.00x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.99x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 10.1 ms: 1.61x faster                                                        |
| django_template | 48.2 ms                                                | 34.5 ms: 1.39x faster                                                        |
| genshi_text     | 31.8 ms                                                | 24.7 ms: 1.29x faster                                                        |
| genshi_xml      | 66.0 ms                                                | 55.0 ms: 1.20x faster                                                        |
| Geometric mean  | (ref)                                                  | 1.37x faster                                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 107 us: 5.09x faster                                                         |
| generators               | 80.1 ms                                                | 33.6 ms: 2.38x faster                                                        |
| deltablue                | 7.91 ms                                                | 3.80 ms: 2.08x faster                                                        |
| crypto_pyaes             | 128 ms                                                 | 66.1 ms: 1.93x faster                                                        |
| logging_silent           | 190 ns                                                 | 100.0 ns: 1.90x faster                                                       |
| spectral_norm            | 170 ms                                                 | 92.2 ms: 1.84x faster                                                        |
| chaos                    | 115 ms                                                 | 63.0 ms: 1.83x faster                                                        |
| richards_super           | 94.7 ms                                                | 53.7 ms: 1.76x faster                                                        |
| raytrace                 | 507 ms                                                 | 293 ms: 1.73x faster                                                         |
| comprehensions           | 28.8 us                                                | 16.7 us: 1.72x faster                                                        |
| pylint                   | 551 ms                                                 | 321 ms: 1.72x faster                                                         |
| richards                 | 79.3 ms                                                | 46.7 ms: 1.70x faster                                                        |
| sqlglot_parse            | 2.17 ms                                                | 1.31 ms: 1.66x faster                                                        |
| hexiom                   | 10.4 ms                                                | 6.29 ms: 1.65x faster                                                        |
| scimark_monte_carlo      | 118 ms                                                 | 71.6 ms: 1.65x faster                                                        |
| mako                     | 16.3 ms                                                | 10.1 ms: 1.61x faster                                                        |
| deepcopy_memo            | 58.5 us                                                | 36.6 us: 1.60x faster                                                        |
| tomli_loads              | 3.14 sec                                               | 1.98 sec: 1.59x faster                                                       |
| pickle_pure_python       | 484 us                                                 | 308 us: 1.57x faster                                                         |
| asyncio_tcp              | 922 ms                                                 | 591 ms: 1.56x faster                                                         |
| sqlglot_transpile        | 2.57 ms                                                | 1.66 ms: 1.55x faster                                                        |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.19 ms: 1.55x faster                                                        |
| async_tree_none          | 728 ms                                                 | 476 ms: 1.53x faster                                                         |
| go                       | 240 ms                                                 | 158 ms: 1.52x faster                                                         |
| scimark_lu               | 176 ms                                                 | 116 ms: 1.51x faster                                                         |
| scimark_fft              | 466 ms                                                 | 311 ms: 1.50x faster                                                         |
| bench_mp_pool            | 24.0 ms                                                | 16.2 ms: 1.49x faster                                                        |
| fannkuch                 | 532 ms                                                 | 358 ms: 1.48x faster                                                         |
| json_dumps               | 14.2 ms                                                | 9.57 ms: 1.48x faster                                                        |
| scimark_sor              | 220 ms                                                 | 148 ms: 1.48x faster                                                         |
| unpickle_pure_python     | 331 us                                                 | 223 us: 1.48x faster                                                         |
| float                    | 117 ms                                                 | 79.8 ms: 1.47x faster                                                        |
| async_tree_io            | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                       |
| create_gc_cycles         | 1.62 ms                                                | 1.11 ms: 1.46x faster                                                        |
| pyflate                  | 716 ms                                                 | 496 ms: 1.44x faster                                                         |
| nbody                    | 154 ms                                                 | 107 ms: 1.44x faster                                                         |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.43x faster                                                       |
| async_tree_memoization   | 870 ms                                                 | 607 ms: 1.43x faster                                                         |
| regex_compile            | 188 ms                                                 | 134 ms: 1.41x faster                                                         |
| coroutines               | 35.1 ms                                                | 25.0 ms: 1.40x faster                                                        |
| thrift                   | 1.07 ms                                                | 766 us: 1.40x faster                                                         |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 728 ms: 1.40x faster                                                         |
| django_template          | 48.2 ms                                                | 34.5 ms: 1.39x faster                                                        |
| logging_simple           | 8.30 us                                                | 6.00 us: 1.38x faster                                                        |
| deepcopy                 | 479 us                                                 | 347 us: 1.38x faster                                                         |
| logging_format           | 9.09 us                                                | 6.63 us: 1.37x faster                                                        |
| pprint_pformat           | 2.10 sec                                               | 1.55 sec: 1.35x faster                                                       |
| pprint_safe_repr         | 1.02 sec                                               | 757 ms: 1.34x faster                                                         |
| xml_etree_process        | 79.1 ms                                                | 59.3 ms: 1.33x faster                                                        |
| pickle_list              | 5.08 us                                                | 3.83 us: 1.33x faster                                                        |
| deepcopy_reduce          | 4.17 us                                                | 3.16 us: 1.32x faster                                                        |
| chameleon                | 9.68 ms                                                | 7.35 ms: 1.32x faster                                                        |
| sqlglot_normalize        | 143 ms                                                 | 109 ms: 1.31x faster                                                         |
| sympy_sum                | 196 ms                                                 | 151 ms: 1.30x faster                                                         |
| json_loads               | 31.2 us                                                | 24.0 us: 1.30x faster                                                        |
| genshi_text              | 31.8 ms                                                | 24.7 ms: 1.29x faster                                                        |
| sympy_str                | 346 ms                                                 | 276 ms: 1.25x faster                                                         |
| sympy_integrate          | 25.8 ms                                                | 20.9 ms: 1.24x faster                                                        |
| nqueens                  | 106 ms                                                 | 86.2 ms: 1.23x faster                                                        |
| sqlglot_optimize         | 69.2 ms                                                | 56.7 ms: 1.22x faster                                                        |
| json                     | 5.69 ms                                                | 4.67 ms: 1.22x faster                                                        |
| meteor_contest           | 120 ms                                                 | 98.7 ms: 1.21x faster                                                        |
| html5lib                 | 88.9 ms                                                | 73.5 ms: 1.21x faster                                                        |
| regex_dna                | 227 ms                                                 | 188 ms: 1.20x faster                                                         |
| genshi_xml               | 66.0 ms                                                | 55.0 ms: 1.20x faster                                                        |
| sympy_expand             | 566 ms                                                 | 473 ms: 1.20x faster                                                         |
| docutils                 | 3.30 sec                                               | 2.76 sec: 1.19x faster                                                       |
| pycparser                | 1.58 sec                                               | 1.32 sec: 1.19x faster                                                       |
| xml_etree_generate       | 99.4 ms                                                | 85.2 ms: 1.17x faster                                                        |
| 2to3                     | 348 ms                                                 | 304 ms: 1.15x faster                                                         |
| xml_etree_iterparse      | 115 ms                                                 | 101 ms: 1.14x faster                                                         |
| unpickle_list            | 5.20 us                                                | 4.56 us: 1.14x faster                                                        |
| xml_etree_parse          | 168 ms                                                 | 148 ms: 1.13x faster                                                         |
| sqlite_synth             | 3.02 us                                                | 2.68 us: 1.13x faster                                                        |
| regex_v8                 | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                        |
| async_generators         | 444 ms                                                 | 406 ms: 1.09x faster                                                         |
| pickle                   | 10.7 us                                                | 9.82 us: 1.09x faster                                                        |
| dulwich_log              | 84.3 ms                                                | 77.8 ms: 1.08x faster                                                        |
| regex_effbot             | 3.63 ms                                                | 3.42 ms: 1.06x faster                                                        |
| gc_traversal             | 3.62 ms                                                | 3.44 ms: 1.05x faster                                                        |
| mdp                      | 2.85 sec                                               | 2.70 sec: 1.05x faster                                                       |
| unpickle                 | 14.4 us                                                | 13.7 us: 1.05x faster                                                        |
| pickle_dict              | 29.6 us                                                | 28.7 us: 1.03x faster                                                        |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                         |
| coverage                 | 79.4 ms                                                | 81.6 ms: 1.03x slower                                                        |
| telco                    | 7.27 ms                                                | 7.68 ms: 1.06x slower                                                        |
| tornado_http             | 136 ms                                                 | 145 ms: 1.06x slower                                                         |
| dask                     | 441 ms                                                 | 495 ms: 1.12x slower                                                         |
| pathlib                  | 20.5 ms                                                | 24.1 ms: 1.18x slower                                                        |
| asyncio_websockets       | 559 ms                                                 | 720 ms: 1.29x slower                                                         |
| python_startup           | 14.6 ms                                                | 19.3 ms: 1.32x slower                                                        |
| bench_thread_pool        | 986 us                                                 | 1.52 ms: 1.54x slower                                                        |
| unpack_sequence          | 60.0 ns                                                | 107 ns: 1.79x slower                                                         |
| python_startup_no_site   | 5.93 ms                                                | 17.8 ms: 3.00x slower                                                        |
| Geometric mean           | (ref)                                                  | 1.31x faster                                                                 |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, djangocms, flaskblogging, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240316-3.13.0a5+-54ce2b4-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.25x
- 99% likely to have a speedup of 1.23x


# Memory

- memory change: 1.31x