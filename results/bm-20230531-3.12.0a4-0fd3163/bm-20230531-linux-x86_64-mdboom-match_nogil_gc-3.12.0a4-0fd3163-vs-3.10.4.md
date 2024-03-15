
# Results vs. 3.10.4

- fork: mdboom
- ref: match_nogil_gc
- machine: linux-x86_64
- commit hash: 0fd3163
- commit date: 2023-05-31
- overall geometric mean: 1.44x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.37x faster
- Memory change: 1.25x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 245 ms: 1.42x faster                                            |
| chameleon      | 9.68 ms                                                | 6.37 ms: 1.52x faster                                           |
| docutils       | 3.30 sec                                               | 2.15 sec: 1.53x faster                                          |
| html5lib       | 88.9 ms                                                | 57.8 ms: 1.54x faster                                           |
| Geometric mean | (ref)                                                  | 1.50x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_io           | 1.77 sec                                               | 534 ms: 3.31x faster                                            |
| async_tree_none         | 728 ms                                                 | 260 ms: 2.80x faster                                            |
| async_tree_memoization  | 870 ms                                                 | 315 ms: 2.76x faster                                            |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 469 ms: 2.17x faster                                            |
| Geometric mean          | (ref)                                                  | 2.73x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 117 ms                                                 | 60.7 ms: 1.93x faster                                           |
| nbody          | 154 ms                                                 | 92.3 ms: 1.66x faster                                           |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                            |
| Geometric mean | (ref)                                                  | 1.48x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 131 ms: 1.43x faster                                            |
| regex_v8       | 27.8 ms                                                | 22.1 ms: 1.26x faster                                           |
| regex_dna      | 227 ms                                                 | 210 ms: 1.08x faster                                            |
| regex_effbot   | 3.63 ms                                                | 3.46 ms: 1.05x faster                                           |
| Geometric mean | (ref)                                                  | 1.19x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 282 us: 1.72x faster                                            |
| unpickle_pure_python | 331 us                                                 | 198 us: 1.67x faster                                            |
| tomli_loads          | 3.14 sec                                               | 1.98 sec: 1.58x faster                                          |
| xml_etree_process    | 79.1 ms                                                | 51.6 ms: 1.53x faster                                           |
| json_dumps           | 14.2 ms                                                | 9.55 ms: 1.48x faster                                           |
| xml_etree_iterparse  | 115 ms                                                 | 80.9 ms: 1.43x faster                                           |
| xml_etree_parse      | 168 ms                                                 | 122 ms: 1.38x faster                                            |
| xml_etree_generate   | 99.4 ms                                                | 73.4 ms: 1.36x faster                                           |
| json_loads           | 31.2 us                                                | 23.7 us: 1.32x faster                                           |
| pickle_list          | 5.08 us                                                | 4.05 us: 1.25x faster                                           |
| unpickle             | 14.4 us                                                | 13.0 us: 1.10x faster                                           |
| unpickle_list        | 5.20 us                                                | 4.95 us: 1.05x faster                                           |
| pickle               | 10.7 us                                                | 10.2 us: 1.05x faster                                           |
| pickle_dict          | 29.6 us                                                | 31.2 us: 1.06x slower                                           |
| Geometric mean       | (ref)                                                  | 1.33x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.24 ms: 1.77x faster                                           |
| python_startup_no_site | 5.93 ms                                                | 5.93 ms: 1.00x faster                                           |
| Geometric mean         | (ref)                                                  | 1.33x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 9.69 ms: 1.68x faster                                           |
| genshi_text     | 31.8 ms                                                | 20.2 ms: 1.58x faster                                           |
| django_template | 48.2 ms                                                | 32.9 ms: 1.47x faster                                           |
| genshi_xml      | 66.0 ms                                                | 45.9 ms: 1.44x faster                                           |
| Geometric mean  | (ref)                                                  | 1.54x faster                                                    |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230531-linux-x86_64-mdboom-match_nogil_gc-3.12.0a4-0fd3163 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_io            | 1.77 sec                                               | 534 ms: 3.31x faster                                            |
| async_tree_none          | 728 ms                                                 | 260 ms: 2.80x faster                                            |
| async_tree_memoization   | 870 ms                                                 | 315 ms: 2.76x faster                                            |
| deltablue                | 7.91 ms                                                | 3.11 ms: 2.54x faster                                           |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 469 ms: 2.17x faster                                            |
| logging_silent           | 190 ns                                                 | 89.6 ns: 2.12x faster                                           |
| scimark_sor              | 220 ms                                                 | 106 ms: 2.07x faster                                            |
| float                    | 117 ms                                                 | 60.7 ms: 1.93x faster                                           |
| richards                 | 79.3 ms                                                | 42.5 ms: 1.87x faster                                           |
| scimark_monte_carlo      | 118 ms                                                 | 65.2 ms: 1.81x faster                                           |
| asyncio_tcp              | 922 ms                                                 | 511 ms: 1.81x faster                                            |
| spectral_norm            | 170 ms                                                 | 94.7 ms: 1.79x faster                                           |
| richards_super           | 94.7 ms                                                | 52.9 ms: 1.79x faster                                           |
| pyflate                  | 716 ms                                                 | 403 ms: 1.78x faster                                            |
| python_startup           | 14.6 ms                                                | 8.24 ms: 1.77x faster                                           |
| raytrace                 | 507 ms                                                 | 286 ms: 1.77x faster                                            |
| go                       | 240 ms                                                 | 137 ms: 1.75x faster                                            |
| crypto_pyaes             | 128 ms                                                 | 73.7 ms: 1.73x faster                                           |
| deepcopy_memo            | 58.5 us                                                | 33.8 us: 1.73x faster                                           |
| pickle_pure_python       | 484 us                                                 | 282 us: 1.72x faster                                            |
| hexiom                   | 10.4 ms                                                | 6.06 ms: 1.71x faster                                           |
| mako                     | 16.3 ms                                                | 9.69 ms: 1.68x faster                                           |
| chaos                    | 115 ms                                                 | 68.8 ms: 1.68x faster                                           |
| scimark_lu               | 176 ms                                                 | 105 ms: 1.67x faster                                            |
| unpickle_pure_python     | 331 us                                                 | 198 us: 1.67x faster                                            |
| nbody                    | 154 ms                                                 | 92.3 ms: 1.66x faster                                           |
| tomli_loads              | 3.14 sec                                               | 1.98 sec: 1.58x faster                                          |
| genshi_text              | 31.8 ms                                                | 20.2 ms: 1.58x faster                                           |
| sqlglot_parse            | 2.17 ms                                                | 1.38 ms: 1.57x faster                                           |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.12 ms: 1.57x faster                                           |
| sqlglot_transpile        | 2.57 ms                                                | 1.67 ms: 1.55x faster                                           |
| html5lib                 | 88.9 ms                                                | 57.8 ms: 1.54x faster                                           |
| docutils                 | 3.30 sec                                               | 2.15 sec: 1.53x faster                                          |
| xml_etree_process        | 79.1 ms                                                | 51.6 ms: 1.53x faster                                           |
| chameleon                | 9.68 ms                                                | 6.37 ms: 1.52x faster                                           |
| pprint_pformat           | 2.10 sec                                               | 1.39 sec: 1.51x faster                                          |
| scimark_fft              | 466 ms                                                 | 309 ms: 1.51x faster                                            |
| pprint_safe_repr         | 1.02 sec                                               | 676 ms: 1.51x faster                                            |
| pycparser                | 1.58 sec                                               | 1.06 sec: 1.49x faster                                          |
| json_dumps               | 14.2 ms                                                | 9.55 ms: 1.48x faster                                           |
| django_template          | 48.2 ms                                                | 32.9 ms: 1.47x faster                                           |
| deepcopy                 | 479 us                                                 | 332 us: 1.44x faster                                            |
| fannkuch                 | 532 ms                                                 | 368 ms: 1.44x faster                                            |
| genshi_xml               | 66.0 ms                                                | 45.9 ms: 1.44x faster                                           |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.43x faster                                          |
| regex_compile            | 188 ms                                                 | 131 ms: 1.43x faster                                            |
| logging_simple           | 8.30 us                                                | 5.80 us: 1.43x faster                                           |
| xml_etree_iterparse      | 115 ms                                                 | 80.9 ms: 1.43x faster                                           |
| 2to3                     | 348 ms                                                 | 245 ms: 1.42x faster                                            |
| logging_format           | 9.09 us                                                | 6.44 us: 1.41x faster                                           |
| deepcopy_reduce          | 4.17 us                                                | 2.97 us: 1.40x faster                                           |
| dask                     | 441 ms                                                 | 317 ms: 1.39x faster                                            |
| thrift                   | 1.07 ms                                                | 772 us: 1.39x faster                                            |
| xml_etree_parse          | 168 ms                                                 | 122 ms: 1.38x faster                                            |
| unpack_sequence          | 60.0 ns                                                | 43.6 ns: 1.38x faster                                           |
| nqueens                  | 106 ms                                                 | 77.6 ms: 1.36x faster                                           |
| xml_etree_generate       | 99.4 ms                                                | 73.4 ms: 1.36x faster                                           |
| coroutines               | 35.1 ms                                                | 26.1 ms: 1.35x faster                                           |
| sqlglot_optimize         | 69.2 ms                                                | 51.6 ms: 1.34x faster                                           |
| dulwich_log              | 84.3 ms                                                | 63.5 ms: 1.33x faster                                           |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.32x faster                                            |
| json_loads               | 31.2 us                                                | 23.7 us: 1.32x faster                                           |
| async_generators         | 444 ms                                                 | 338 ms: 1.31x faster                                            |
| sympy_integrate          | 25.8 ms                                                | 20.2 ms: 1.28x faster                                           |
| regex_v8                 | 27.8 ms                                                | 22.1 ms: 1.26x faster                                           |
| pickle_list              | 5.08 us                                                | 4.05 us: 1.25x faster                                           |
| bench_thread_pool        | 986 us                                                 | 792 us: 1.25x faster                                            |
| sympy_expand             | 566 ms                                                 | 455 ms: 1.24x faster                                            |
| json                     | 5.69 ms                                                | 4.59 ms: 1.24x faster                                           |
| sympy_str                | 346 ms                                                 | 281 ms: 1.23x faster                                            |
| sympy_sum                | 196 ms                                                 | 163 ms: 1.21x faster                                            |
| comprehensions           | 28.8 us                                                | 23.9 us: 1.20x faster                                           |
| typing_runtime_protocols | 544 us                                                 | 463 us: 1.17x faster                                            |
| djangocms                | 38.4 us                                                | 33.1 us: 1.16x faster                                           |
| mdp                      | 2.85 sec                                               | 2.48 sec: 1.15x faster                                          |
| sqlite_synth             | 3.02 us                                                | 2.67 us: 1.13x faster                                           |
| pathlib                  | 20.5 ms                                                | 18.2 ms: 1.13x faster                                           |
| telco                    | 7.27 ms                                                | 6.52 ms: 1.11x faster                                           |
| create_gc_cycles         | 1.62 ms                                                | 1.46 ms: 1.11x faster                                           |
| unpickle                 | 14.4 us                                                | 13.0 us: 1.10x faster                                           |
| meteor_contest           | 120 ms                                                 | 109 ms: 1.10x faster                                            |
| regex_dna                | 227 ms                                                 | 210 ms: 1.08x faster                                            |
| gc_traversal             | 3.62 ms                                                | 3.38 ms: 1.07x faster                                           |
| unpickle_list            | 5.20 us                                                | 4.95 us: 1.05x faster                                           |
| regex_effbot             | 3.63 ms                                                | 3.46 ms: 1.05x faster                                           |
| pickle                   | 10.7 us                                                | 10.2 us: 1.05x faster                                           |
| generators               | 80.1 ms                                                | 79.1 ms: 1.01x faster                                           |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                            |
| python_startup_no_site   | 5.93 ms                                                | 5.93 ms: 1.00x faster                                           |
| pickle_dict              | 29.6 us                                                | 31.2 us: 1.06x slower                                           |
| coverage                 | 79.4 ms                                                | 99.2 ms: 1.25x slower                                           |
| Geometric mean           | (ref)                                                  | 1.44x faster                                                    |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (9) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.42x
- 95% likely to have a speedup of 1.40x
- 99% likely to have a speedup of 1.37x


# Memory

- memory change: 1.25x