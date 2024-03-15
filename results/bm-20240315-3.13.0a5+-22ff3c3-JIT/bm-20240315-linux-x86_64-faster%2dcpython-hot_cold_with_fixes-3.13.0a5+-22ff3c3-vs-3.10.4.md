# Results vs. 3.10.4

- fork: faster-cpython
- ref: hot_cold_with_fixes
- machine: linux-x86_64
- commit hash: 22ff3c3
- commit date: 2024-03-15
- overall geometric mean: 1.29x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.22x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 281 ms: 1.24x faster                                                            |
| chameleon      | 9.68 ms                                                | 7.17 ms: 1.35x faster                                                           |
| docutils       | 3.30 sec                                               | 2.77 sec: 1.19x faster                                                          |
| html5lib       | 88.9 ms                                                | 66.1 ms: 1.34x faster                                                           |
| tornado_http   | 136 ms                                                 | 99.3 ms: 1.37x faster                                                           |
| Geometric mean | (ref)                                                  | 1.30x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 446 ms: 1.63x faster                                                            |
| async_tree_memoization  | 870 ms                                                 | 578 ms: 1.50x faster                                                            |
| async_tree_io           | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                          |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 722 ms: 1.41x faster                                                            |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 92.7 ms: 1.66x faster                                                           |
| float          | 117 ms                                                 | 80.7 ms: 1.45x faster                                                           |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                  | 1.34x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 145 ms: 1.30x faster                                                            |
| regex_v8       | 27.8 ms                                                | 24.9 ms: 1.11x faster                                                           |
| regex_dna      | 227 ms                                                 | 228 ms: 1.00x slower                                                            |
| regex_effbot   | 3.63 ms                                                | 3.69 ms: 1.02x slower                                                           |
| Geometric mean | (ref)                                                  | 1.09x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 312 us: 1.55x faster                                                            |
| tomli_loads          | 3.14 sec                                               | 2.07 sec: 1.52x faster                                                          |
| unpickle_pure_python | 331 us                                                 | 238 us: 1.39x faster                                                            |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                           |
| xml_etree_process    | 79.1 ms                                                | 61.1 ms: 1.30x faster                                                           |
| xml_etree_generate   | 99.4 ms                                                | 88.6 ms: 1.12x faster                                                           |
| json_loads           | 31.2 us                                                | 28.9 us: 1.08x faster                                                           |
| xml_etree_iterparse  | 115 ms                                                 | 108 ms: 1.07x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 160 ms: 1.05x faster                                                            |
| unpickle_list        | 5.20 us                                                | 4.99 us: 1.04x faster                                                           |
| pickle_list          | 5.08 us                                                | 5.26 us: 1.04x slower                                                           |
| unpickle             | 14.4 us                                                | 15.4 us: 1.07x slower                                                           |
| pickle               | 10.7 us                                                | 12.1 us: 1.13x slower                                                           |
| pickle_dict          | 29.6 us                                                | 34.7 us: 1.17x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.13x faster                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 11.3 ms: 1.29x faster                                                           |
| python_startup_no_site | 5.93 ms                                                | 9.93 ms: 1.67x slower                                                           |
| Geometric mean         | (ref)                                                  | 1.14x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 11.2 ms: 1.46x faster                                                           |
| django_template | 48.2 ms                                                | 34.6 ms: 1.39x faster                                                           |
| genshi_text     | 31.8 ms                                                | 25.6 ms: 1.24x faster                                                           |
| genshi_xml      | 66.0 ms                                                | 56.8 ms: 1.16x faster                                                           |
| Geometric mean  | (ref)                                                  | 1.31x faster                                                                    |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|--------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 113 us: 4.83x faster                                                            |
| generators               | 80.1 ms                                                | 30.3 ms: 2.64x faster                                                           |
| deltablue                | 7.91 ms                                                | 3.52 ms: 2.25x faster                                                           |
| logging_silent           | 190 ns                                                 | 101 ns: 1.88x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 506 ms: 1.82x faster                                                            |
| chaos                    | 115 ms                                                 | 63.6 ms: 1.82x faster                                                           |
| richards_super           | 94.7 ms                                                | 54.0 ms: 1.75x faster                                                           |
| raytrace                 | 507 ms                                                 | 290 ms: 1.75x faster                                                            |
| crypto_pyaes             | 128 ms                                                 | 74.6 ms: 1.71x faster                                                           |
| scimark_monte_carlo      | 118 ms                                                 | 69.8 ms: 1.69x faster                                                           |
| richards                 | 79.3 ms                                                | 46.9 ms: 1.69x faster                                                           |
| pylint                   | 551 ms                                                 | 326 ms: 1.69x faster                                                            |
| nbody                    | 154 ms                                                 | 92.7 ms: 1.66x faster                                                           |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.64x faster                                                           |
| async_tree_none          | 728 ms                                                 | 446 ms: 1.63x faster                                                            |
| scimark_sor              | 220 ms                                                 | 135 ms: 1.62x faster                                                            |
| comprehensions           | 28.8 us                                                | 17.9 us: 1.61x faster                                                           |
| coroutines               | 35.1 ms                                                | 22.5 ms: 1.56x faster                                                           |
| pickle_pure_python       | 484 us                                                 | 312 us: 1.55x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.67 ms: 1.54x faster                                                           |
| tomli_loads              | 3.14 sec                                               | 2.07 sec: 1.52x faster                                                          |
| spectral_norm            | 170 ms                                                 | 113 ms: 1.51x faster                                                            |
| async_tree_memoization   | 870 ms                                                 | 578 ms: 1.50x faster                                                            |
| go                       | 240 ms                                                 | 160 ms: 1.50x faster                                                            |
| pyflate                  | 716 ms                                                 | 479 ms: 1.50x faster                                                            |
| deepcopy_memo            | 58.5 us                                                | 39.1 us: 1.49x faster                                                           |
| mako                     | 16.3 ms                                                | 11.2 ms: 1.46x faster                                                           |
| async_tree_io            | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                          |
| float                    | 117 ms                                                 | 80.7 ms: 1.45x faster                                                           |
| hexiom                   | 10.4 ms                                                | 7.17 ms: 1.45x faster                                                           |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 722 ms: 1.41x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.84 sec: 1.40x faster                                                          |
| logging_simple           | 8.30 us                                                | 5.95 us: 1.40x faster                                                           |
| django_template          | 48.2 ms                                                | 34.6 ms: 1.39x faster                                                           |
| unpickle_pure_python     | 331 us                                                 | 238 us: 1.39x faster                                                            |
| logging_format           | 9.09 us                                                | 6.60 us: 1.38x faster                                                           |
| tornado_http             | 136 ms                                                 | 99.3 ms: 1.37x faster                                                           |
| scimark_fft              | 466 ms                                                 | 342 ms: 1.36x faster                                                            |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                           |
| chameleon                | 9.68 ms                                                | 7.17 ms: 1.35x faster                                                           |
| pprint_pformat           | 2.10 sec                                               | 1.56 sec: 1.35x faster                                                          |
| html5lib                 | 88.9 ms                                                | 66.1 ms: 1.34x faster                                                           |
| pprint_safe_repr         | 1.02 sec                                               | 759 ms: 1.34x faster                                                            |
| deepcopy                 | 479 us                                                 | 358 us: 1.34x faster                                                            |
| thrift                   | 1.07 ms                                                | 801 us: 1.34x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.13 us: 1.33x faster                                                           |
| scimark_lu               | 176 ms                                                 | 133 ms: 1.32x faster                                                            |
| fannkuch                 | 532 ms                                                 | 403 ms: 1.32x faster                                                            |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.93 ms: 1.31x faster                                                           |
| sqlglot_normalize        | 143 ms                                                 | 110 ms: 1.30x faster                                                            |
| regex_compile            | 188 ms                                                 | 145 ms: 1.30x faster                                                            |
| xml_etree_process        | 79.1 ms                                                | 61.1 ms: 1.30x faster                                                           |
| pycparser                | 1.58 sec                                               | 1.22 sec: 1.29x faster                                                          |
| python_startup           | 14.6 ms                                                | 11.3 ms: 1.29x faster                                                           |
| genshi_text              | 31.8 ms                                                | 25.6 ms: 1.24x faster                                                           |
| 2to3                     | 348 ms                                                 | 281 ms: 1.24x faster                                                            |
| sympy_sum                | 196 ms                                                 | 161 ms: 1.22x faster                                                            |
| djangocms                | 38.4 us                                                | 31.6 us: 1.21x faster                                                           |
| sqlglot_optimize         | 69.2 ms                                                | 57.2 ms: 1.21x faster                                                           |
| sympy_integrate          | 25.8 ms                                                | 21.4 ms: 1.21x faster                                                           |
| sympy_str                | 346 ms                                                 | 289 ms: 1.20x faster                                                            |
| aiohttp                  | 1.44 ms                                                | 1.20 ms: 1.20x faster                                                           |
| dulwich_log              | 84.3 ms                                                | 70.5 ms: 1.20x faster                                                           |
| docutils                 | 3.30 sec                                               | 2.77 sec: 1.19x faster                                                          |
| gunicorn                 | 1.53 ms                                                | 1.30 ms: 1.18x faster                                                           |
| dask                     | 441 ms                                                 | 376 ms: 1.17x faster                                                            |
| genshi_xml               | 66.0 ms                                                | 56.8 ms: 1.16x faster                                                           |
| nqueens                  | 106 ms                                                 | 91.1 ms: 1.16x faster                                                           |
| sympy_expand             | 566 ms                                                 | 489 ms: 1.16x faster                                                            |
| bench_thread_pool        | 986 us                                                 | 869 us: 1.13x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 88.6 ms: 1.12x faster                                                           |
| regex_v8                 | 27.8 ms                                                | 24.9 ms: 1.11x faster                                                           |
| pathlib                  | 20.5 ms                                                | 18.8 ms: 1.09x faster                                                           |
| json                     | 5.69 ms                                                | 5.25 ms: 1.08x faster                                                           |
| json_loads               | 31.2 us                                                | 28.9 us: 1.08x faster                                                           |
| mdp                      | 2.85 sec                                               | 2.64 sec: 1.08x faster                                                          |
| meteor_contest           | 120 ms                                                 | 111 ms: 1.07x faster                                                            |
| xml_etree_iterparse      | 115 ms                                                 | 108 ms: 1.07x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.53 ms: 1.06x faster                                                           |
| sqlite_synth             | 3.02 us                                                | 2.86 us: 1.06x faster                                                           |
| xml_etree_parse          | 168 ms                                                 | 160 ms: 1.05x faster                                                            |
| unpickle_list            | 5.20 us                                                | 4.99 us: 1.04x faster                                                           |
| gc_traversal             | 3.62 ms                                                | 3.57 ms: 1.02x faster                                                           |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                            |
| regex_dna                | 227 ms                                                 | 228 ms: 1.00x slower                                                            |
| asyncio_websockets       | 559 ms                                                 | 564 ms: 1.01x slower                                                            |
| regex_effbot             | 3.63 ms                                                | 3.69 ms: 1.02x slower                                                           |
| bench_mp_pool            | 24.0 ms                                                | 24.8 ms: 1.03x slower                                                           |
| pickle_list              | 5.08 us                                                | 5.26 us: 1.04x slower                                                           |
| async_generators         | 444 ms                                                 | 475 ms: 1.07x slower                                                            |
| unpickle                 | 14.4 us                                                | 15.4 us: 1.07x slower                                                           |
| pickle                   | 10.7 us                                                | 12.1 us: 1.13x slower                                                           |
| telco                    | 7.27 ms                                                | 8.47 ms: 1.17x slower                                                           |
| pickle_dict              | 29.6 us                                                | 34.7 us: 1.17x slower                                                           |
| coverage                 | 79.4 ms                                                | 96.9 ms: 1.22x slower                                                           |
| unpack_sequence          | 60.0 ns                                                | 85.2 ns: 1.42x slower                                                           |
| python_startup_no_site   | 5.93 ms                                                | 9.93 ms: 1.67x slower                                                           |
| Geometric mean           | (ref)                                                  | 1.29x faster                                                                    |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240315-3.13.0a5+-22ff3c3-JIT/bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.25x
- 95% likely to have a speedup of 1.24x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.22x