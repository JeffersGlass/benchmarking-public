
# Results vs. 3.10.4

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: fe6f94a
- commit date: 2024-02-08
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.14x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 288 ms: 1.21x faster                                                           |
| chameleon      | 9.68 ms                                                | 7.37 ms: 1.31x faster                                                          |
| docutils       | 3.30 sec                                               | 2.71 sec: 1.22x faster                                                         |
| tornado_http   | 136 ms                                                 | 99.4 ms: 1.37x faster                                                          |
| Geometric mean | (ref)                                                  | 1.28x faster                                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 457 ms: 1.59x faster                                                           |
| async_tree_memoization  | 870 ms                                                 | 582 ms: 1.49x faster                                                           |
| async_tree_io           | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                         |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 727 ms: 1.40x faster                                                           |
| Geometric mean          | (ref)                                                  | 1.49x faster                                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| float          | 117 ms                                                 | 105 ms: 1.11x faster                                                           |
| nbody          | 154 ms                                                 | 141 ms: 1.09x faster                                                           |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                           |
| Geometric mean | (ref)                                                  | 1.07x faster                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 157 ms: 1.20x faster                                                           |
| regex_v8       | 27.8 ms                                                | 24.4 ms: 1.14x faster                                                          |
| regex_dna      | 227 ms                                                 | 225 ms: 1.01x faster                                                           |
| regex_effbot   | 3.63 ms                                                | 3.70 ms: 1.02x slower                                                          |
| Geometric mean | (ref)                                                  | 1.08x faster                                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 301 us: 1.61x faster                                                           |
| unpickle_pure_python | 331 us                                                 | 240 us: 1.38x faster                                                           |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                          |
| xml_etree_process    | 79.1 ms                                                | 61.8 ms: 1.28x faster                                                          |
| json_loads           | 31.2 us                                                | 27.8 us: 1.12x faster                                                          |
| tomli_loads          | 3.14 sec                                               | 2.84 sec: 1.11x faster                                                         |
| xml_etree_generate   | 99.4 ms                                                | 91.3 ms: 1.09x faster                                                          |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                                           |
| pickle_list          | 5.08 us                                                | 5.24 us: 1.03x slower                                                          |
| unpickle             | 14.4 us                                                | 15.2 us: 1.06x slower                                                          |
| pickle               | 10.7 us                                                | 11.9 us: 1.11x slower                                                          |
| pickle_dict          | 29.6 us                                                | 35.3 us: 1.19x slower                                                          |
| Geometric mean       | (ref)                                                  | 1.10x faster                                                                   |

Benchmark hidden because not significant (2): unpickle_list, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                          |
| python_startup_no_site | 5.93 ms                                                | 8.81 ms: 1.48x slower                                                          |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 15.4 ms: 1.06x faster                                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 119 us: 4.58x faster                                                           |
| generators               | 80.1 ms                                                | 29.6 ms: 2.71x faster                                                          |
| deltablue                | 7.91 ms                                                | 3.63 ms: 2.18x faster                                                          |
| asyncio_tcp              | 922 ms                                                 | 490 ms: 1.88x faster                                                           |
| logging_silent           | 190 ns                                                 | 106 ns: 1.79x faster                                                           |
| scimark_sor              | 220 ms                                                 | 124 ms: 1.77x faster                                                           |
| richards_super           | 94.7 ms                                                | 56.8 ms: 1.67x faster                                                          |
| raytrace                 | 507 ms                                                 | 312 ms: 1.63x faster                                                           |
| pickle_pure_python       | 484 us                                                 | 301 us: 1.61x faster                                                           |
| async_tree_none          | 728 ms                                                 | 457 ms: 1.59x faster                                                           |
| sqlglot_parse            | 2.17 ms                                                | 1.37 ms: 1.59x faster                                                          |
| richards                 | 79.3 ms                                                | 50.2 ms: 1.58x faster                                                          |
| coroutines               | 35.1 ms                                                | 22.9 ms: 1.53x faster                                                          |
| sqlglot_transpile        | 2.57 ms                                                | 1.70 ms: 1.51x faster                                                          |
| async_tree_memoization   | 870 ms                                                 | 582 ms: 1.49x faster                                                           |
| scimark_lu               | 176 ms                                                 | 119 ms: 1.47x faster                                                           |
| async_tree_io            | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                         |
| chaos                    | 115 ms                                                 | 79.8 ms: 1.45x faster                                                          |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                          |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.81 sec: 1.42x faster                                                         |
| deepcopy_memo            | 58.5 us                                                | 41.2 us: 1.42x faster                                                          |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 727 ms: 1.40x faster                                                           |
| unpickle_pure_python     | 331 us                                                 | 240 us: 1.38x faster                                                           |
| tornado_http             | 136 ms                                                 | 99.4 ms: 1.37x faster                                                          |
| crypto_pyaes             | 128 ms                                                 | 93.8 ms: 1.36x faster                                                          |
| logging_simple           | 8.30 us                                                | 6.10 us: 1.36x faster                                                          |
| go                       | 240 ms                                                 | 177 ms: 1.36x faster                                                           |
| deepcopy                 | 479 us                                                 | 356 us: 1.34x faster                                                           |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                          |
| deepcopy_reduce          | 4.17 us                                                | 3.12 us: 1.34x faster                                                          |
| scimark_monte_carlo      | 118 ms                                                 | 89.8 ms: 1.32x faster                                                          |
| chameleon                | 9.68 ms                                                | 7.37 ms: 1.31x faster                                                          |
| logging_format           | 9.09 us                                                | 6.94 us: 1.31x faster                                                          |
| pycparser                | 1.58 sec                                               | 1.23 sec: 1.28x faster                                                         |
| xml_etree_process        | 79.1 ms                                                | 61.8 ms: 1.28x faster                                                          |
| pyflate                  | 716 ms                                                 | 573 ms: 1.25x faster                                                           |
| sqlglot_normalize        | 143 ms                                                 | 117 ms: 1.23x faster                                                           |
| pprint_safe_repr         | 1.02 sec                                               | 834 ms: 1.22x faster                                                           |
| dulwich_log              | 84.3 ms                                                | 69.3 ms: 1.22x faster                                                          |
| docutils                 | 3.30 sec                                               | 2.71 sec: 1.22x faster                                                         |
| 2to3                     | 348 ms                                                 | 288 ms: 1.21x faster                                                           |
| comprehensions           | 28.8 us                                                | 23.9 us: 1.20x faster                                                          |
| pprint_pformat           | 2.10 sec                                               | 1.75 sec: 1.20x faster                                                         |
| regex_compile            | 188 ms                                                 | 157 ms: 1.20x faster                                                           |
| dask                     | 441 ms                                                 | 369 ms: 1.20x faster                                                           |
| sympy_sum                | 196 ms                                                 | 165 ms: 1.19x faster                                                           |
| sympy_integrate          | 25.8 ms                                                | 21.7 ms: 1.19x faster                                                          |
| sqlglot_optimize         | 69.2 ms                                                | 59.0 ms: 1.17x faster                                                          |
| sympy_str                | 346 ms                                                 | 299 ms: 1.15x faster                                                           |
| bench_thread_pool        | 986 us                                                 | 855 us: 1.15x faster                                                           |
| sympy_expand             | 566 ms                                                 | 495 ms: 1.14x faster                                                           |
| regex_v8                 | 27.8 ms                                                | 24.4 ms: 1.14x faster                                                          |
| json_loads               | 31.2 us                                                | 27.8 us: 1.12x faster                                                          |
| float                    | 117 ms                                                 | 105 ms: 1.11x faster                                                           |
| tomli_loads              | 3.14 sec                                               | 2.84 sec: 1.11x faster                                                         |
| json                     | 5.69 ms                                                | 5.15 ms: 1.11x faster                                                          |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                                          |
| unpack_sequence          | 60.0 ns                                                | 54.6 ns: 1.10x faster                                                          |
| pathlib                  | 20.5 ms                                                | 18.7 ms: 1.09x faster                                                          |
| nbody                    | 154 ms                                                 | 141 ms: 1.09x faster                                                           |
| xml_etree_generate       | 99.4 ms                                                | 91.3 ms: 1.09x faster                                                          |
| fannkuch                 | 532 ms                                                 | 490 ms: 1.09x faster                                                           |
| hexiom                   | 10.4 ms                                                | 9.60 ms: 1.08x faster                                                          |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                                           |
| mako                     | 16.3 ms                                                | 15.4 ms: 1.06x faster                                                          |
| sqlite_synth             | 3.02 us                                                | 2.90 us: 1.04x faster                                                          |
| spectral_norm            | 170 ms                                                 | 167 ms: 1.02x faster                                                           |
| meteor_contest           | 120 ms                                                 | 118 ms: 1.02x faster                                                           |
| nqueens                  | 106 ms                                                 | 104 ms: 1.01x faster                                                           |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                           |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                           |
| regex_dna                | 227 ms                                                 | 225 ms: 1.01x faster                                                           |
| mdp                      | 2.85 sec                                               | 2.83 sec: 1.01x faster                                                         |
| regex_effbot             | 3.63 ms                                                | 3.70 ms: 1.02x slower                                                          |
| gc_traversal             | 3.62 ms                                                | 3.70 ms: 1.02x slower                                                          |
| async_generators         | 444 ms                                                 | 456 ms: 1.03x slower                                                           |
| pickle_list              | 5.08 us                                                | 5.24 us: 1.03x slower                                                          |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 6.74 ms: 1.04x slower                                                          |
| unpickle                 | 14.4 us                                                | 15.2 us: 1.06x slower                                                          |
| scimark_fft              | 466 ms                                                 | 496 ms: 1.06x slower                                                           |
| pickle                   | 10.7 us                                                | 11.9 us: 1.11x slower                                                          |
| coverage                 | 79.4 ms                                                | 94.7 ms: 1.19x slower                                                          |
| pickle_dict              | 29.6 us                                                | 35.3 us: 1.19x slower                                                          |
| telco                    | 7.27 ms                                                | 8.95 ms: 1.23x slower                                                          |
| python_startup_no_site   | 5.93 ms                                                | 8.81 ms: 1.48x slower                                                          |
| Geometric mean           | (ref)                                                  | 1.23x faster                                                                   |

Benchmark hidden because not significant (4): mypy2, unpickle_list, xml_etree_iterparse, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240208-3.13.0a3+-fe6f94a-PYTHON_UOPS/bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.16x
- 99% likely to have a speedup of 1.14x


# Memory

- memory change: 1.06x