
# Results vs. 3.10.4

- fork: mdboom
- ref: nogil_d595911
- machine: linux-x86_64
- commit hash: d595911
- commit date: 2023-04-27
- overall geometric mean: 1.18x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.14x faster
- Memory change: 1.47x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 303 ms: 1.15x faster                                                 |
| chameleon      | 9.44 ms                                                      | 8.37 ms: 1.13x faster                                                |
| docutils       | 3.41 sec                                                     | 2.99 sec: 1.14x faster                                               |
| html5lib       | 94.6 ms                                                      | 73.1 ms: 1.29x faster                                                |
| Geometric mean | (ref)                                                        | 1.18x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 595 ms: 2.69x faster                                                 |
| async_tree_none         | 692 ms                                                       | 304 ms: 2.28x faster                                                 |
| async_tree_memoization  | 819 ms                                                       | 361 ms: 2.27x faster                                                 |
| async_tree_cpu_io_mixed | 936 ms                                                       | 529 ms: 1.77x faster                                                 |
| Geometric mean          | (ref)                                                        | 2.23x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 111 ms                                                       | 65.5 ms: 1.70x faster                                                |
| nbody          | 134 ms                                                       | 102 ms: 1.32x faster                                                 |
| pidigits       | 271 ms                                                       | 246 ms: 1.10x faster                                                 |
| Geometric mean | (ref)                                                        | 1.35x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 157 ms: 1.21x faster                                                 |
| regex_v8       | 27.2 ms                                                      | 23.1 ms: 1.18x faster                                                |
| regex_dna      | 261 ms                                                       | 233 ms: 1.12x faster                                                 |
| regex_effbot   | 3.09 ms                                                      | 3.30 ms: 1.07x slower                                                |
| Geometric mean | (ref)                                                        | 1.11x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 329 us: 1.38x faster                                                 |
| unpickle_pure_python | 312 us                                                       | 233 us: 1.34x faster                                                 |
| json_dumps           | 14.5 ms                                                      | 11.4 ms: 1.27x faster                                                |
| xml_etree_process    | 75.9 ms                                                      | 62.8 ms: 1.21x faster                                                |
| tomli_loads          | 2.92 sec                                                     | 2.49 sec: 1.17x faster                                               |
| xml_etree_parse      | 160 ms                                                       | 137 ms: 1.17x faster                                                 |
| xml_etree_generate   | 92.3 ms                                                      | 85.4 ms: 1.08x faster                                                |
| pickle               | 9.89 us                                                      | 9.64 us: 1.03x faster                                                |
| json_loads           | 30.3 us                                                      | 32.3 us: 1.06x slower                                                |
| unpickle_list        | 4.65 us                                                      | 5.01 us: 1.08x slower                                                |
| pickle_list          | 4.12 us                                                      | 4.46 us: 1.08x slower                                                |
| pickle_dict          | 29.5 us                                                      | 32.7 us: 1.11x slower                                                |
| xml_etree_iterparse  | 110 ms                                                       | 126 ms: 1.14x slower                                                 |
| unpickle             | 13.5 us                                                      | 15.8 us: 1.17x slower                                                |
| Geometric mean       | (ref)                                                        | 1.06x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup_no_site | 7.33 ms                                                      | 8.45 ms: 1.15x slower                                                |
| Geometric mean         | (ref)                                                        | 1.07x slower                                                         |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|-----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| django_template | 50.2 ms                                                      | 40.6 ms: 1.24x faster                                                |
| genshi_text     | 31.4 ms                                                      | 27.0 ms: 1.17x faster                                                |
| genshi_xml      | 63.3 ms                                                      | 54.6 ms: 1.16x faster                                                |
| mako            | 14.7 ms                                                      | 14.9 ms: 1.01x slower                                                |
| Geometric mean  | (ref)                                                        | 1.13x faster                                                         |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_io            | 1.60 sec                                                     | 595 ms: 2.69x faster                                                 |
| async_tree_none          | 692 ms                                                       | 304 ms: 2.28x faster                                                 |
| async_tree_memoization   | 819 ms                                                       | 361 ms: 2.27x faster                                                 |
| asyncio_tcp              | 779 ms                                                       | 399 ms: 1.95x faster                                                 |
| deltablue                | 7.50 ms                                                      | 4.00 ms: 1.88x faster                                                |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.70 sec: 1.82x faster                                               |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 529 ms: 1.77x faster                                                 |
| float                    | 111 ms                                                       | 65.5 ms: 1.70x faster                                                |
| logging_silent           | 167 ns                                                       | 99.0 ns: 1.69x faster                                                |
| go                       | 262 ms                                                       | 169 ms: 1.55x faster                                                 |
| scimark_lu               | 167 ms                                                       | 108 ms: 1.54x faster                                                 |
| scimark_sor              | 180 ms                                                       | 117 ms: 1.54x faster                                                 |
| pyflate                  | 733 ms                                                       | 482 ms: 1.52x faster                                                 |
| richards                 | 75.1 ms                                                      | 53.5 ms: 1.40x faster                                                |
| chaos                    | 109 ms                                                       | 77.8 ms: 1.40x faster                                                |
| pickle_pure_python       | 455 us                                                       | 329 us: 1.38x faster                                                 |
| pycparser                | 1.67 sec                                                     | 1.22 sec: 1.37x faster                                               |
| richards_super           | 90.6 ms                                                      | 66.5 ms: 1.36x faster                                                |
| hexiom                   | 9.42 ms                                                      | 7.01 ms: 1.34x faster                                                |
| crypto_pyaes             | 119 ms                                                       | 88.9 ms: 1.34x faster                                                |
| unpickle_pure_python     | 312 us                                                       | 233 us: 1.34x faster                                                 |
| spectral_norm            | 139 ms                                                       | 105 ms: 1.33x faster                                                 |
| nbody                    | 134 ms                                                       | 102 ms: 1.32x faster                                                 |
| raytrace                 | 489 ms                                                       | 376 ms: 1.30x faster                                                 |
| scimark_monte_carlo      | 107 ms                                                       | 82.9 ms: 1.30x faster                                                |
| html5lib                 | 94.6 ms                                                      | 73.1 ms: 1.29x faster                                                |
| sqlglot_parse            | 2.24 ms                                                      | 1.73 ms: 1.29x faster                                                |
| sqlglot_transpile        | 2.68 ms                                                      | 2.08 ms: 1.29x faster                                                |
| json_dumps               | 14.5 ms                                                      | 11.4 ms: 1.27x faster                                                |
| async_generators         | 421 ms                                                       | 335 ms: 1.26x faster                                                 |
| django_template          | 50.2 ms                                                      | 40.6 ms: 1.24x faster                                                |
| thrift                   | 1.18 ms                                                      | 957 us: 1.23x faster                                                 |
| deepcopy_memo            | 49.8 us                                                      | 41.0 us: 1.22x faster                                                |
| logging_simple           | 8.88 us                                                      | 7.32 us: 1.21x faster                                                |
| regex_compile            | 190 ms                                                       | 157 ms: 1.21x faster                                                 |
| xml_etree_process        | 75.9 ms                                                      | 62.8 ms: 1.21x faster                                                |
| dulwich_log              | 81.1 ms                                                      | 67.2 ms: 1.21x faster                                                |
| pprint_safe_repr         | 1.05 sec                                                     | 871 ms: 1.20x faster                                                 |
| pprint_pformat           | 2.15 sec                                                     | 1.81 sec: 1.19x faster                                               |
| logging_format           | 9.64 us                                                      | 8.16 us: 1.18x faster                                                |
| regex_v8                 | 27.2 ms                                                      | 23.1 ms: 1.18x faster                                                |
| sqlglot_optimize         | 70.1 ms                                                      | 59.9 ms: 1.17x faster                                                |
| tomli_loads              | 2.92 sec                                                     | 2.49 sec: 1.17x faster                                               |
| sqlglot_normalize        | 144 ms                                                       | 123 ms: 1.17x faster                                                 |
| xml_etree_parse          | 160 ms                                                       | 137 ms: 1.17x faster                                                 |
| genshi_text              | 31.4 ms                                                      | 27.0 ms: 1.17x faster                                                |
| deepcopy                 | 468 us                                                       | 403 us: 1.16x faster                                                 |
| genshi_xml               | 63.3 ms                                                      | 54.6 ms: 1.16x faster                                                |
| 2to3                     | 350 ms                                                       | 303 ms: 1.15x faster                                                 |
| nqueens                  | 115 ms                                                       | 99.8 ms: 1.15x faster                                                |
| unpack_sequence          | 59.9 ns                                                      | 52.4 ns: 1.14x faster                                                |
| docutils                 | 3.41 sec                                                     | 2.99 sec: 1.14x faster                                               |
| chameleon                | 9.44 ms                                                      | 8.37 ms: 1.13x faster                                                |
| regex_dna                | 261 ms                                                       | 233 ms: 1.12x faster                                                 |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.58 ms: 1.11x faster                                                |
| gc_traversal             | 3.42 ms                                                      | 3.08 ms: 1.11x faster                                                |
| scimark_fft              | 361 ms                                                       | 327 ms: 1.11x faster                                                 |
| pidigits                 | 271 ms                                                       | 246 ms: 1.10x faster                                                 |
| xml_etree_generate       | 92.3 ms                                                      | 85.4 ms: 1.08x faster                                                |
| fannkuch                 | 483 ms                                                       | 447 ms: 1.08x faster                                                 |
| coroutines               | 30.3 ms                                                      | 28.1 ms: 1.08x faster                                                |
| pathlib                  | 21.4 ms                                                      | 19.8 ms: 1.08x faster                                                |
| deepcopy_reduce          | 4.01 us                                                      | 3.74 us: 1.07x faster                                                |
| sympy_expand             | 600 ms                                                       | 562 ms: 1.07x faster                                                 |
| mdp                      | 3.01 sec                                                     | 2.82 sec: 1.07x faster                                               |
| sympy_integrate          | 28.2 ms                                                      | 26.4 ms: 1.07x faster                                                |
| sympy_str                | 360 ms                                                       | 344 ms: 1.05x faster                                                 |
| sqlite_synth             | 2.99 us                                                      | 2.88 us: 1.04x faster                                                |
| pickle                   | 9.89 us                                                      | 9.64 us: 1.03x faster                                                |
| sympy_sum                | 193 ms                                                       | 191 ms: 1.01x faster                                                 |
| mako                     | 14.7 ms                                                      | 14.9 ms: 1.01x slower                                                |
| json_loads               | 30.3 us                                                      | 32.3 us: 1.06x slower                                                |
| regex_effbot             | 3.09 ms                                                      | 3.30 ms: 1.07x slower                                                |
| typing_runtime_protocols | 537 us                                                       | 575 us: 1.07x slower                                                 |
| json                     | 5.86 ms                                                      | 6.28 ms: 1.07x slower                                                |
| unpickle_list            | 4.65 us                                                      | 5.01 us: 1.08x slower                                                |
| pickle_list              | 4.12 us                                                      | 4.46 us: 1.08x slower                                                |
| generators               | 57.3 ms                                                      | 62.3 ms: 1.09x slower                                                |
| create_gc_cycles         | 1.76 ms                                                      | 1.93 ms: 1.10x slower                                                |
| meteor_contest           | 138 ms                                                       | 153 ms: 1.11x slower                                                 |
| pickle_dict              | 29.5 us                                                      | 32.7 us: 1.11x slower                                                |
| comprehensions           | 26.7 us                                                      | 29.6 us: 1.11x slower                                                |
| xml_etree_iterparse      | 110 ms                                                       | 126 ms: 1.14x slower                                                 |
| python_startup_no_site   | 7.33 ms                                                      | 8.45 ms: 1.15x slower                                                |
| unpickle                 | 13.5 us                                                      | 15.8 us: 1.17x slower                                                |
| bench_mp_pool            | 6.37 ms                                                      | 7.77 ms: 1.22x slower                                                |
| coverage                 | 63.3 ms                                                      | 97.6 ms: 1.54x slower                                                |
| bench_thread_pool        | 1.14 ms                                                      | 2.03 ms: 1.78x slower                                                |
| Geometric mean           | (ref)                                                        | 1.18x faster                                                         |

Benchmark hidden because not significant (2): python_startup, telco
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_websockets, dask, flaskblogging, gunicorn, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.16x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.14x


# Memory

- memory change: 1.47x