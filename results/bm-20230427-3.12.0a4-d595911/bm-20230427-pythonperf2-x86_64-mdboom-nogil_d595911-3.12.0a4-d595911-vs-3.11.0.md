
# Results vs. 3.11.0

- fork: mdboom
- ref: nogil_d595911
- machine: linux-x86_64
- commit hash: d595911
- commit date: 2023-04-27
- overall geometric mean: 1.03x slower \*
- HPT reliability: 99.99%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.36x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 303 ms: 1.06x slower                                                 |
| chameleon      | 7.92 ms                                                      | 8.37 ms: 1.06x slower                                                |
| docutils       | 2.85 sec                                                     | 2.99 sec: 1.05x slower                                               |
| html5lib       | 72.2 ms                                                      | 73.1 ms: 1.01x slower                                                |
| Geometric mean | (ref)                                                        | 1.04x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_io           | 1.17 sec                                                     | 595 ms: 1.97x faster                                                 |
| async_tree_memoization  | 629 ms                                                       | 361 ms: 1.74x faster                                                 |
| async_tree_none         | 518 ms                                                       | 304 ms: 1.70x faster                                                 |
| async_tree_cpu_io_mixed | 753 ms                                                       | 529 ms: 1.42x faster                                                 |
| Geometric mean          | (ref)                                                        | 1.70x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 74.9 ms                                                      | 65.5 ms: 1.14x faster                                                |
| pidigits       | 251 ms                                                       | 246 ms: 1.02x faster                                                 |
| nbody          | 92.9 ms                                                      | 102 ms: 1.10x slower                                                 |
| Geometric mean | (ref)                                                        | 1.02x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_v8       | 24.4 ms                                                      | 23.1 ms: 1.06x faster                                                |
| regex_effbot   | 3.34 ms                                                      | 3.30 ms: 1.01x faster                                                |
| regex_compile  | 156 ms                                                       | 157 ms: 1.01x slower                                                 |
| regex_dna      | 227 ms                                                       | 233 ms: 1.02x slower                                                 |
| Geometric mean | (ref)                                                        | 1.01x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 11.4 ms: 1.16x faster                                                |
| xml_etree_parse      | 155 ms                                                       | 137 ms: 1.13x faster                                                 |
| pickle               | 9.89 us                                                      | 9.64 us: 1.03x faster                                                |
| unpickle_pure_python | 238 us                                                       | 233 us: 1.02x faster                                                 |
| pickle_dict          | 32.3 us                                                      | 32.7 us: 1.01x slower                                                |
| pickle_pure_python   | 316 us                                                       | 329 us: 1.04x slower                                                 |
| xml_etree_generate   | 79.7 ms                                                      | 85.4 ms: 1.07x slower                                                |
| unpickle_list        | 4.60 us                                                      | 5.01 us: 1.09x slower                                                |
| tomli_loads          | 2.25 sec                                                     | 2.49 sec: 1.11x slower                                               |
| json_loads           | 28.9 us                                                      | 32.3 us: 1.12x slower                                                |
| xml_etree_process    | 55.9 ms                                                      | 62.8 ms: 1.12x slower                                                |
| pickle_list          | 3.94 us                                                      | 4.46 us: 1.13x slower                                                |
| xml_etree_iterparse  | 107 ms                                                       | 126 ms: 1.18x slower                                                 |
| unpickle             | 13.3 us                                                      | 15.8 us: 1.19x slower                                                |
| Geometric mean       | (ref)                                                        | 1.05x slower                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 11.5 ms: 1.07x slower                                                |
| python_startup_no_site | 7.73 ms                                                      | 8.45 ms: 1.09x slower                                                |
| Geometric mean         | (ref)                                                        | 1.08x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|-----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| genshi_xml      | 57.1 ms                                                      | 54.6 ms: 1.05x faster                                                |
| django_template | 39.3 ms                                                      | 40.6 ms: 1.03x slower                                                |
| genshi_text     | 25.5 ms                                                      | 27.0 ms: 1.06x slower                                                |
| mako            | 11.0 ms                                                      | 14.9 ms: 1.36x slower                                                |
| Geometric mean  | (ref)                                                        | 1.09x slower                                                         |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_io            | 1.17 sec                                                     | 595 ms: 1.97x faster                                                 |
| asyncio_tcp              | 747 ms                                                       | 399 ms: 1.87x faster                                                 |
| asyncio_tcp_ssl          | 3.07 sec                                                     | 1.70 sec: 1.80x faster                                               |
| async_tree_memoization   | 629 ms                                                       | 361 ms: 1.74x faster                                                 |
| async_tree_none          | 518 ms                                                       | 304 ms: 1.70x faster                                                 |
| async_tree_cpu_io_mixed  | 753 ms                                                       | 529 ms: 1.42x faster                                                 |
| gc_traversal             | 4.15 ms                                                      | 3.08 ms: 1.35x faster                                                |
| json_dumps               | 13.3 ms                                                      | 11.4 ms: 1.16x faster                                                |
| float                    | 74.9 ms                                                      | 65.5 ms: 1.14x faster                                                |
| xml_etree_parse          | 155 ms                                                       | 137 ms: 1.13x faster                                                 |
| pycparser                | 1.31 sec                                                     | 1.22 sec: 1.07x faster                                               |
| regex_v8                 | 24.4 ms                                                      | 23.1 ms: 1.06x faster                                                |
| scimark_lu               | 114 ms                                                       | 108 ms: 1.06x faster                                                 |
| genshi_xml               | 57.1 ms                                                      | 54.6 ms: 1.05x faster                                                |
| nqueens                  | 103 ms                                                       | 99.8 ms: 1.03x faster                                                |
| pickle                   | 9.89 us                                                      | 9.64 us: 1.03x faster                                                |
| unpickle_pure_python     | 238 us                                                       | 233 us: 1.02x faster                                                 |
| pidigits                 | 251 ms                                                       | 246 ms: 1.02x faster                                                 |
| logging_silent           | 100 ns                                                       | 99.0 ns: 1.01x faster                                                |
| regex_effbot             | 3.34 ms                                                      | 3.30 ms: 1.01x faster                                                |
| hexiom                   | 6.98 ms                                                      | 7.01 ms: 1.00x slower                                                |
| regex_compile            | 156 ms                                                       | 157 ms: 1.01x slower                                                 |
| deltablue                | 3.97 ms                                                      | 4.00 ms: 1.01x slower                                                |
| logging_simple           | 7.24 us                                                      | 7.32 us: 1.01x slower                                                |
| coroutines               | 27.8 ms                                                      | 28.1 ms: 1.01x slower                                                |
| pickle_dict              | 32.3 us                                                      | 32.7 us: 1.01x slower                                                |
| html5lib                 | 72.2 ms                                                      | 73.1 ms: 1.01x slower                                                |
| sqlglot_normalize        | 122 ms                                                       | 123 ms: 1.01x slower                                                 |
| sqlglot_optimize         | 59.0 ms                                                      | 59.9 ms: 1.02x slower                                                |
| sympy_expand             | 553 ms                                                       | 562 ms: 1.02x slower                                                 |
| mdp                      | 2.77 sec                                                     | 2.82 sec: 1.02x slower                                               |
| sympy_str                | 337 ms                                                       | 344 ms: 1.02x slower                                                 |
| regex_dna                | 227 ms                                                       | 233 ms: 1.02x slower                                                 |
| sympy_integrate          | 25.8 ms                                                      | 26.4 ms: 1.03x slower                                                |
| thrift                   | 931 us                                                       | 957 us: 1.03x slower                                                 |
| deepcopy                 | 391 us                                                       | 403 us: 1.03x slower                                                 |
| sympy_sum                | 186 ms                                                       | 191 ms: 1.03x slower                                                 |
| django_template          | 39.3 ms                                                      | 40.6 ms: 1.03x slower                                                |
| chaos                    | 74.9 ms                                                      | 77.8 ms: 1.04x slower                                                |
| pickle_pure_python       | 316 us                                                       | 329 us: 1.04x slower                                                 |
| async_generators         | 322 ms                                                       | 335 ms: 1.04x slower                                                 |
| richards_super           | 63.6 ms                                                      | 66.5 ms: 1.05x slower                                                |
| pathlib                  | 18.9 ms                                                      | 19.8 ms: 1.05x slower                                                |
| docutils                 | 2.85 sec                                                     | 2.99 sec: 1.05x slower                                               |
| chameleon                | 7.92 ms                                                      | 8.37 ms: 1.06x slower                                                |
| 2to3                     | 287 ms                                                       | 303 ms: 1.06x slower                                                 |
| logging_format           | 7.71 us                                                      | 8.16 us: 1.06x slower                                                |
| genshi_text              | 25.5 ms                                                      | 27.0 ms: 1.06x slower                                                |
| crypto_pyaes             | 83.3 ms                                                      | 88.9 ms: 1.07x slower                                                |
| scimark_sor              | 110 ms                                                       | 117 ms: 1.07x slower                                                 |
| telco                    | 6.81 ms                                                      | 7.29 ms: 1.07x slower                                                |
| go                       | 158 ms                                                       | 169 ms: 1.07x slower                                                 |
| python_startup           | 10.7 ms                                                      | 11.5 ms: 1.07x slower                                                |
| xml_etree_generate       | 79.7 ms                                                      | 85.4 ms: 1.07x slower                                                |
| pyflate                  | 449 ms                                                       | 482 ms: 1.07x slower                                                 |
| fannkuch                 | 416 ms                                                       | 447 ms: 1.08x slower                                                 |
| richards                 | 49.7 ms                                                      | 53.5 ms: 1.08x slower                                                |
| typing_runtime_protocols | 532 us                                                       | 575 us: 1.08x slower                                                 |
| pprint_safe_repr         | 805 ms                                                       | 871 ms: 1.08x slower                                                 |
| pprint_pformat           | 1.67 sec                                                     | 1.81 sec: 1.08x slower                                               |
| sqlglot_transpile        | 1.91 ms                                                      | 2.08 ms: 1.09x slower                                                |
| unpickle_list            | 4.60 us                                                      | 5.01 us: 1.09x slower                                                |
| deepcopy_memo            | 37.5 us                                                      | 41.0 us: 1.09x slower                                                |
| python_startup_no_site   | 7.73 ms                                                      | 8.45 ms: 1.09x slower                                                |
| nbody                    | 92.9 ms                                                      | 102 ms: 1.10x slower                                                 |
| deepcopy_reduce          | 3.40 us                                                      | 3.74 us: 1.10x slower                                                |
| spectral_norm            | 95.1 ms                                                      | 105 ms: 1.10x slower                                                 |
| tomli_loads              | 2.25 sec                                                     | 2.49 sec: 1.11x slower                                               |
| json_loads               | 28.9 us                                                      | 32.3 us: 1.12x slower                                                |
| xml_etree_process        | 55.9 ms                                                      | 62.8 ms: 1.12x slower                                                |
| json                     | 5.58 ms                                                      | 6.28 ms: 1.13x slower                                                |
| scimark_sparse_mat_mult  | 4.06 ms                                                      | 4.58 ms: 1.13x slower                                                |
| pickle_list              | 3.94 us                                                      | 4.46 us: 1.13x slower                                                |
| generators               | 54.6 ms                                                      | 62.3 ms: 1.14x slower                                                |
| sqlite_synth             | 2.52 us                                                      | 2.88 us: 1.14x slower                                                |
| sqlglot_parse            | 1.51 ms                                                      | 1.73 ms: 1.14x slower                                                |
| unpack_sequence          | 45.7 ns                                                      | 52.4 ns: 1.15x slower                                                |
| scimark_fft              | 281 ms                                                       | 327 ms: 1.16x slower                                                 |
| meteor_contest           | 131 ms                                                       | 153 ms: 1.17x slower                                                 |
| xml_etree_iterparse      | 107 ms                                                       | 126 ms: 1.18x slower                                                 |
| comprehensions           | 25.1 us                                                      | 29.6 us: 1.18x slower                                                |
| scimark_monte_carlo      | 69.8 ms                                                      | 82.9 ms: 1.19x slower                                                |
| unpickle                 | 13.3 us                                                      | 15.8 us: 1.19x slower                                                |
| raytrace                 | 309 ms                                                       | 376 ms: 1.21x slower                                                 |
| create_gc_cycles         | 1.58 ms                                                      | 1.93 ms: 1.23x slower                                                |
| mako                     | 11.0 ms                                                      | 14.9 ms: 1.36x slower                                                |
| coverage                 | 66.1 ms                                                      | 97.6 ms: 1.48x slower                                                |
| bench_mp_pool            | 4.70 ms                                                      | 7.77 ms: 1.65x slower                                                |
| bench_thread_pool        | 1.00 ms                                                      | 2.03 ms: 2.03x slower                                                |
| Geometric mean           | (ref)                                                        | 1.03x slower                                                         |

Benchmark hidden because not significant (1): dulwich_log
Ignored benchmarks (14) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, dask, flaskblogging, gunicorn, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http


# HPT report

- Reliability score: 99.99% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.36x