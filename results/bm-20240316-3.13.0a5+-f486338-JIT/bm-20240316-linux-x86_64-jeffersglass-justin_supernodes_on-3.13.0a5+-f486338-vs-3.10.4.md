# Results vs. 3.10.4

- fork: jeffersglass
- ref: justin_supernodes_on
- machine: linux-x86_64
- commit hash: f486338
- commit date: 2024-03-16
- overall geometric mean: 1.33x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.25x faster
- Memory change: 1.32x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 299 ms: 1.16x faster                                                         |
| chameleon      | 9.68 ms                                                | 7.13 ms: 1.36x faster                                                        |
| docutils       | 3.30 sec                                               | 2.64 sec: 1.25x faster                                                       |
| html5lib       | 88.9 ms                                                | 70.4 ms: 1.26x faster                                                        |
| tornado_http   | 136 ms                                                 | 144 ms: 1.06x slower                                                         |
| Geometric mean | (ref)                                                  | 1.19x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 467 ms: 1.56x faster                                                         |
| async_tree_io           | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                       |
| async_tree_memoization  | 870 ms                                                 | 610 ms: 1.43x faster                                                         |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 724 ms: 1.40x faster                                                         |
| Geometric mean          | (ref)                                                  | 1.46x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 103 ms: 1.49x faster                                                         |
| float          | 117 ms                                                 | 79.2 ms: 1.48x faster                                                        |
| pidigits       | 191 ms                                                 | 186 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                  | 1.31x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 133 ms: 1.41x faster                                                         |
| regex_dna      | 227 ms                                                 | 197 ms: 1.15x faster                                                         |
| regex_v8       | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                        |
| regex_effbot   | 3.63 ms                                                | 3.42 ms: 1.06x faster                                                        |
| Geometric mean | (ref)                                                  | 1.18x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| tomli_loads          | 3.14 sec                                               | 1.93 sec: 1.63x faster                                                       |
| pickle_pure_python   | 484 us                                                 | 312 us: 1.55x faster                                                         |
| unpickle_pure_python | 331 us                                                 | 223 us: 1.48x faster                                                         |
| json_dumps           | 14.2 ms                                                | 9.63 ms: 1.47x faster                                                        |
| pickle_list          | 5.08 us                                                | 3.76 us: 1.35x faster                                                        |
| xml_etree_process    | 79.1 ms                                                | 58.6 ms: 1.35x faster                                                        |
| json_loads           | 31.2 us                                                | 24.1 us: 1.30x faster                                                        |
| xml_etree_generate   | 99.4 ms                                                | 84.1 ms: 1.18x faster                                                        |
| xml_etree_iterparse  | 115 ms                                                 | 97.9 ms: 1.18x faster                                                        |
| unpickle_list        | 5.20 us                                                | 4.49 us: 1.16x faster                                                        |
| xml_etree_parse      | 168 ms                                                 | 152 ms: 1.11x faster                                                         |
| pickle               | 10.7 us                                                | 9.69 us: 1.10x faster                                                        |
| unpickle             | 14.4 us                                                | 13.3 us: 1.08x faster                                                        |
| pickle_dict          | 29.6 us                                                | 27.5 us: 1.07x faster                                                        |
| Geometric mean       | (ref)                                                  | 1.27x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 18.3 ms: 1.26x slower                                                        |
| python_startup_no_site | 5.93 ms                                                | 16.8 ms: 2.83x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.89x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 9.84 ms: 1.66x faster                                                        |
| django_template | 48.2 ms                                                | 34.5 ms: 1.40x faster                                                        |
| genshi_text     | 31.8 ms                                                | 25.0 ms: 1.27x faster                                                        |
| genshi_xml      | 66.0 ms                                                | 54.3 ms: 1.22x faster                                                        |
| Geometric mean  | (ref)                                                  | 1.38x faster                                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 106 us: 5.13x faster                                                         |
| generators               | 80.1 ms                                                | 31.6 ms: 2.53x faster                                                        |
| deltablue                | 7.91 ms                                                | 3.71 ms: 2.13x faster                                                        |
| crypto_pyaes             | 128 ms                                                 | 65.4 ms: 1.95x faster                                                        |
| chaos                    | 115 ms                                                 | 61.3 ms: 1.88x faster                                                        |
| logging_silent           | 190 ns                                                 | 102 ns: 1.87x faster                                                         |
| spectral_norm            | 170 ms                                                 | 91.5 ms: 1.86x faster                                                        |
| raytrace                 | 507 ms                                                 | 280 ms: 1.81x faster                                                         |
| richards_super           | 94.7 ms                                                | 52.7 ms: 1.80x faster                                                        |
| pylint                   | 551 ms                                                 | 309 ms: 1.78x faster                                                         |
| comprehensions           | 28.8 us                                                | 16.5 us: 1.74x faster                                                        |
| richards                 | 79.3 ms                                                | 45.6 ms: 1.74x faster                                                        |
| scimark_monte_carlo      | 118 ms                                                 | 68.5 ms: 1.73x faster                                                        |
| sqlglot_parse            | 2.17 ms                                                | 1.30 ms: 1.67x faster                                                        |
| hexiom                   | 10.4 ms                                                | 6.24 ms: 1.67x faster                                                        |
| mako                     | 16.3 ms                                                | 9.84 ms: 1.66x faster                                                        |
| tomli_loads              | 3.14 sec                                               | 1.93 sec: 1.63x faster                                                       |
| deepcopy_memo            | 58.5 us                                                | 36.6 us: 1.60x faster                                                        |
| pyflate                  | 716 ms                                                 | 449 ms: 1.60x faster                                                         |
| sqlglot_transpile        | 2.57 ms                                                | 1.62 ms: 1.59x faster                                                        |
| asyncio_tcp              | 922 ms                                                 | 584 ms: 1.58x faster                                                         |
| async_tree_none          | 728 ms                                                 | 467 ms: 1.56x faster                                                         |
| pickle_pure_python       | 484 us                                                 | 312 us: 1.55x faster                                                         |
| bench_mp_pool            | 24.0 ms                                                | 15.6 ms: 1.54x faster                                                        |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.21 ms: 1.54x faster                                                        |
| scimark_fft              | 466 ms                                                 | 304 ms: 1.53x faster                                                         |
| fannkuch                 | 532 ms                                                 | 349 ms: 1.52x faster                                                         |
| go                       | 240 ms                                                 | 159 ms: 1.51x faster                                                         |
| nbody                    | 154 ms                                                 | 103 ms: 1.49x faster                                                         |
| scimark_sor              | 220 ms                                                 | 148 ms: 1.49x faster                                                         |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.74 sec: 1.48x faster                                                       |
| unpickle_pure_python     | 331 us                                                 | 223 us: 1.48x faster                                                         |
| scimark_lu               | 176 ms                                                 | 119 ms: 1.48x faster                                                         |
| float                    | 117 ms                                                 | 79.2 ms: 1.48x faster                                                        |
| json_dumps               | 14.2 ms                                                | 9.63 ms: 1.47x faster                                                        |
| create_gc_cycles         | 1.62 ms                                                | 1.10 ms: 1.47x faster                                                        |
| async_tree_io            | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                       |
| async_tree_memoization   | 870 ms                                                 | 610 ms: 1.43x faster                                                         |
| regex_compile            | 188 ms                                                 | 133 ms: 1.41x faster                                                         |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 724 ms: 1.40x faster                                                         |
| deepcopy                 | 479 us                                                 | 343 us: 1.40x faster                                                         |
| django_template          | 48.2 ms                                                | 34.5 ms: 1.40x faster                                                        |
| thrift                   | 1.07 ms                                                | 771 us: 1.39x faster                                                         |
| logging_simple           | 8.30 us                                                | 6.03 us: 1.38x faster                                                        |
| logging_format           | 9.09 us                                                | 6.62 us: 1.37x faster                                                        |
| pprint_pformat           | 2.10 sec                                               | 1.55 sec: 1.36x faster                                                       |
| chameleon                | 9.68 ms                                                | 7.13 ms: 1.36x faster                                                        |
| pprint_safe_repr         | 1.02 sec                                               | 750 ms: 1.36x faster                                                         |
| pickle_list              | 5.08 us                                                | 3.76 us: 1.35x faster                                                        |
| xml_etree_process        | 79.1 ms                                                | 58.6 ms: 1.35x faster                                                        |
| coroutines               | 35.1 ms                                                | 26.2 ms: 1.34x faster                                                        |
| deepcopy_reduce          | 4.17 us                                                | 3.14 us: 1.33x faster                                                        |
| sympy_sum                | 196 ms                                                 | 148 ms: 1.33x faster                                                         |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.32x faster                                                         |
| json_loads               | 31.2 us                                                | 24.1 us: 1.30x faster                                                        |
| sympy_str                | 346 ms                                                 | 269 ms: 1.29x faster                                                         |
| genshi_text              | 31.8 ms                                                | 25.0 ms: 1.27x faster                                                        |
| html5lib                 | 88.9 ms                                                | 70.4 ms: 1.26x faster                                                        |
| sympy_integrate          | 25.8 ms                                                | 20.6 ms: 1.26x faster                                                        |
| pycparser                | 1.58 sec                                               | 1.26 sec: 1.25x faster                                                       |
| docutils                 | 3.30 sec                                               | 2.64 sec: 1.25x faster                                                       |
| sqlglot_optimize         | 69.2 ms                                                | 55.8 ms: 1.24x faster                                                        |
| json                     | 5.69 ms                                                | 4.60 ms: 1.24x faster                                                        |
| sympy_expand             | 566 ms                                                 | 457 ms: 1.24x faster                                                         |
| genshi_xml               | 66.0 ms                                                | 54.3 ms: 1.22x faster                                                        |
| nqueens                  | 106 ms                                                 | 87.6 ms: 1.21x faster                                                        |
| mdp                      | 2.85 sec                                               | 2.39 sec: 1.19x faster                                                       |
| meteor_contest           | 120 ms                                                 | 101 ms: 1.19x faster                                                         |
| xml_etree_generate       | 99.4 ms                                                | 84.1 ms: 1.18x faster                                                        |
| xml_etree_iterparse      | 115 ms                                                 | 97.9 ms: 1.18x faster                                                        |
| 2to3                     | 348 ms                                                 | 299 ms: 1.16x faster                                                         |
| unpickle_list            | 5.20 us                                                | 4.49 us: 1.16x faster                                                        |
| regex_dna                | 227 ms                                                 | 197 ms: 1.15x faster                                                         |
| sqlite_synth             | 3.02 us                                                | 2.66 us: 1.14x faster                                                        |
| regex_v8                 | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                        |
| async_generators         | 444 ms                                                 | 400 ms: 1.11x faster                                                         |
| xml_etree_parse          | 168 ms                                                 | 152 ms: 1.11x faster                                                         |
| pickle                   | 10.7 us                                                | 9.69 us: 1.10x faster                                                        |
| unpickle                 | 14.4 us                                                | 13.3 us: 1.08x faster                                                        |
| dulwich_log              | 84.3 ms                                                | 78.0 ms: 1.08x faster                                                        |
| pickle_dict              | 29.6 us                                                | 27.5 us: 1.07x faster                                                        |
| regex_effbot             | 3.63 ms                                                | 3.42 ms: 1.06x faster                                                        |
| pidigits                 | 191 ms                                                 | 186 ms: 1.02x faster                                                         |
| gc_traversal             | 3.62 ms                                                | 3.68 ms: 1.02x slower                                                        |
| coverage                 | 79.4 ms                                                | 81.5 ms: 1.03x slower                                                        |
| telco                    | 7.27 ms                                                | 7.66 ms: 1.05x slower                                                        |
| tornado_http             | 136 ms                                                 | 144 ms: 1.06x slower                                                         |
| dask                     | 441 ms                                                 | 472 ms: 1.07x slower                                                         |
| pathlib                  | 20.5 ms                                                | 23.9 ms: 1.17x slower                                                        |
| python_startup           | 14.6 ms                                                | 18.3 ms: 1.26x slower                                                        |
| asyncio_websockets       | 559 ms                                                 | 721 ms: 1.29x slower                                                         |
| bench_thread_pool        | 986 us                                                 | 1.49 ms: 1.51x slower                                                        |
| unpack_sequence          | 60.0 ns                                                | 104 ns: 1.74x slower                                                         |
| python_startup_no_site   | 5.93 ms                                                | 16.8 ms: 2.83x slower                                                        |
| Geometric mean           | (ref)                                                  | 1.33x faster                                                                 |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, djangocms, flaskblogging, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240316-3.13.0a5+-f486338-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.29x
- 95% likely to have a speedup of 1.28x
- 99% likely to have a speedup of 1.25x


# Memory

- memory change: 1.32x