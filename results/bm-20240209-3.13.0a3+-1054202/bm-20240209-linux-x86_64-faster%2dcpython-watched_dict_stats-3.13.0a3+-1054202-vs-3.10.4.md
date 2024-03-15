
# Results vs. 3.10.4

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: 1054202
- commit date: 2024-02-09
- overall geometric mean: 1.36x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.29x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 264 ms: 1.32x faster                                                           |
| chameleon      | 9.68 ms                                                | 6.92 ms: 1.40x faster                                                          |
| docutils       | 3.30 sec                                               | 2.59 sec: 1.27x faster                                                         |
| tornado_http   | 136 ms                                                 | 94.4 ms: 1.44x faster                                                          |
| Geometric mean | (ref)                                                  | 1.36x faster                                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 433 ms: 1.68x faster                                                           |
| async_tree_memoization  | 870 ms                                                 | 560 ms: 1.55x faster                                                           |
| async_tree_io           | 1.77 sec                                               | 1.17 sec: 1.52x faster                                                         |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 702 ms: 1.45x faster                                                           |
| Geometric mean          | (ref)                                                  | 1.55x faster                                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 90.3 ms: 1.70x faster                                                          |
| float          | 117 ms                                                 | 80.5 ms: 1.45x faster                                                          |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                           |
| Geometric mean | (ref)                                                  | 1.36x faster                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 130 ms: 1.45x faster                                                           |
| regex_v8       | 27.8 ms                                                | 25.0 ms: 1.11x faster                                                          |
| regex_dna      | 227 ms                                                 | 220 ms: 1.03x faster                                                           |
| Geometric mean | (ref)                                                  | 1.14x faster                                                                   |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 296 us: 1.64x faster                                                           |
| unpickle_pure_python | 331 us                                                 | 212 us: 1.56x faster                                                           |
| tomli_loads          | 3.14 sec                                               | 2.12 sec: 1.48x faster                                                         |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                          |
| xml_etree_process    | 79.1 ms                                                | 58.3 ms: 1.36x faster                                                          |
| xml_etree_generate   | 99.4 ms                                                | 85.8 ms: 1.16x faster                                                          |
| json_loads           | 31.2 us                                                | 28.2 us: 1.11x faster                                                          |
| xml_etree_iterparse  | 115 ms                                                 | 105 ms: 1.10x faster                                                           |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.08x faster                                                           |
| unpickle_list        | 5.20 us                                                | 5.02 us: 1.04x faster                                                          |
| pickle_list          | 5.08 us                                                | 5.04 us: 1.01x faster                                                          |
| unpickle             | 14.4 us                                                | 15.4 us: 1.07x slower                                                          |
| pickle               | 10.7 us                                                | 11.4 us: 1.07x slower                                                          |
| pickle_dict          | 29.6 us                                                | 33.0 us: 1.11x slower                                                          |
| Geometric mean       | (ref)                                                  | 1.17x faster                                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.44x faster                                                          |
| python_startup_no_site | 5.93 ms                                                | 8.77 ms: 1.48x slower                                                          |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.2 ms: 1.46x faster                                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 109 us: 4.99x faster                                                           |
| generators               | 80.1 ms                                                | 29.3 ms: 2.73x faster                                                          |
| deltablue                | 7.91 ms                                                | 3.22 ms: 2.46x faster                                                          |
| chaos                    | 115 ms                                                 | 58.2 ms: 1.98x faster                                                          |
| raytrace                 | 507 ms                                                 | 258 ms: 1.97x faster                                                           |
| logging_silent           | 190 ns                                                 | 98.5 ns: 1.93x faster                                                          |
| asyncio_tcp              | 922 ms                                                 | 485 ms: 1.90x faster                                                           |
| crypto_pyaes             | 128 ms                                                 | 70.3 ms: 1.82x faster                                                          |
| richards_super           | 94.7 ms                                                | 52.7 ms: 1.80x faster                                                          |
| comprehensions           | 28.8 us                                                | 16.1 us: 1.79x faster                                                          |
| scimark_monte_carlo      | 118 ms                                                 | 66.6 ms: 1.77x faster                                                          |
| go                       | 240 ms                                                 | 138 ms: 1.74x faster                                                           |
| hexiom                   | 10.4 ms                                                | 6.01 ms: 1.73x faster                                                          |
| sqlglot_parse            | 2.17 ms                                                | 1.26 ms: 1.72x faster                                                          |
| scimark_sor              | 220 ms                                                 | 129 ms: 1.70x faster                                                           |
| nbody                    | 154 ms                                                 | 90.3 ms: 1.70x faster                                                          |
| async_tree_none          | 728 ms                                                 | 433 ms: 1.68x faster                                                           |
| richards                 | 79.3 ms                                                | 47.5 ms: 1.67x faster                                                          |
| pickle_pure_python       | 484 us                                                 | 296 us: 1.64x faster                                                           |
| sqlglot_transpile        | 2.57 ms                                                | 1.57 ms: 1.64x faster                                                          |
| coroutines               | 35.1 ms                                                | 22.0 ms: 1.60x faster                                                          |
| scimark_lu               | 176 ms                                                 | 111 ms: 1.59x faster                                                           |
| deepcopy_memo            | 58.5 us                                                | 37.4 us: 1.56x faster                                                          |
| unpickle_pure_python     | 331 us                                                 | 212 us: 1.56x faster                                                           |
| async_tree_memoization   | 870 ms                                                 | 560 ms: 1.55x faster                                                           |
| spectral_norm            | 170 ms                                                 | 109 ms: 1.55x faster                                                           |
| pyflate                  | 716 ms                                                 | 467 ms: 1.53x faster                                                           |
| async_tree_io            | 1.77 sec                                               | 1.17 sec: 1.52x faster                                                         |
| logging_simple           | 8.30 us                                                | 5.58 us: 1.49x faster                                                          |
| tomli_loads              | 3.14 sec                                               | 2.12 sec: 1.48x faster                                                         |
| logging_format           | 9.09 us                                                | 6.15 us: 1.48x faster                                                          |
| mako                     | 16.3 ms                                                | 11.2 ms: 1.46x faster                                                          |
| regex_compile            | 188 ms                                                 | 130 ms: 1.45x faster                                                           |
| float                    | 117 ms                                                 | 80.5 ms: 1.45x faster                                                          |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 702 ms: 1.45x faster                                                           |
| tornado_http             | 136 ms                                                 | 94.4 ms: 1.44x faster                                                          |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.44x faster                                                         |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.44x faster                                                          |
| pprint_pformat           | 2.10 sec                                               | 1.50 sec: 1.40x faster                                                         |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.62 ms: 1.40x faster                                                          |
| deepcopy                 | 479 us                                                 | 342 us: 1.40x faster                                                           |
| chameleon                | 9.68 ms                                                | 6.92 ms: 1.40x faster                                                          |
| pprint_safe_repr         | 1.02 sec                                               | 728 ms: 1.40x faster                                                           |
| deepcopy_reduce          | 4.17 us                                                | 3.02 us: 1.38x faster                                                          |
| pycparser                | 1.58 sec                                               | 1.16 sec: 1.36x faster                                                         |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                          |
| xml_etree_process        | 79.1 ms                                                | 58.3 ms: 1.36x faster                                                          |
| fannkuch                 | 532 ms                                                 | 392 ms: 1.36x faster                                                           |
| unpack_sequence          | 60.0 ns                                                | 44.6 ns: 1.35x faster                                                          |
| scimark_fft              | 466 ms                                                 | 348 ms: 1.34x faster                                                           |
| sympy_sum                | 196 ms                                                 | 148 ms: 1.32x faster                                                           |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.32x faster                                                           |
| 2to3                     | 348 ms                                                 | 264 ms: 1.32x faster                                                           |
| sympy_integrate          | 25.8 ms                                                | 19.6 ms: 1.31x faster                                                          |
| nqueens                  | 106 ms                                                 | 80.9 ms: 1.31x faster                                                          |
| dulwich_log              | 84.3 ms                                                | 65.7 ms: 1.28x faster                                                          |
| sqlglot_optimize         | 69.2 ms                                                | 54.1 ms: 1.28x faster                                                          |
| sympy_str                | 346 ms                                                 | 271 ms: 1.28x faster                                                           |
| docutils                 | 3.30 sec                                               | 2.59 sec: 1.27x faster                                                         |
| sympy_expand             | 566 ms                                                 | 458 ms: 1.24x faster                                                           |
| dask                     | 441 ms                                                 | 362 ms: 1.22x faster                                                           |
| bench_thread_pool        | 986 us                                                 | 820 us: 1.20x faster                                                           |
| xml_etree_generate       | 99.4 ms                                                | 85.8 ms: 1.16x faster                                                          |
| pathlib                  | 20.5 ms                                                | 18.1 ms: 1.13x faster                                                          |
| mdp                      | 2.85 sec                                               | 2.53 sec: 1.12x faster                                                         |
| meteor_contest           | 120 ms                                                 | 107 ms: 1.12x faster                                                           |
| regex_v8                 | 27.8 ms                                                | 25.0 ms: 1.11x faster                                                          |
| json                     | 5.69 ms                                                | 5.14 ms: 1.11x faster                                                          |
| json_loads               | 31.2 us                                                | 28.2 us: 1.11x faster                                                          |
| xml_etree_iterparse      | 115 ms                                                 | 105 ms: 1.10x faster                                                           |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.09x faster                                                          |
| xml_etree_parse          | 168 ms                                                 | 156 ms: 1.08x faster                                                           |
| sqlite_synth             | 3.02 us                                                | 2.82 us: 1.07x faster                                                          |
| unpickle_list            | 5.20 us                                                | 5.02 us: 1.04x faster                                                          |
| regex_dna                | 227 ms                                                 | 220 ms: 1.03x faster                                                           |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                           |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                           |
| pickle_list              | 5.08 us                                                | 5.04 us: 1.01x faster                                                          |
| async_generators         | 444 ms                                                 | 450 ms: 1.01x slower                                                           |
| gc_traversal             | 3.62 ms                                                | 3.74 ms: 1.03x slower                                                          |
| unpickle                 | 14.4 us                                                | 15.4 us: 1.07x slower                                                          |
| pickle                   | 10.7 us                                                | 11.4 us: 1.07x slower                                                          |
| pickle_dict              | 29.6 us                                                | 33.0 us: 1.11x slower                                                          |
| telco                    | 7.27 ms                                                | 8.37 ms: 1.15x slower                                                          |
| coverage                 | 79.4 ms                                                | 94.2 ms: 1.19x slower                                                          |
| python_startup_no_site   | 5.93 ms                                                | 8.77 ms: 1.48x slower                                                          |
| Geometric mean           | (ref)                                                  | 1.36x faster                                                                   |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240209-3.13.0a3+-1054202/bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.32x
- 95% likely to have a speedup of 1.31x
- 99% likely to have a speedup of 1.29x


# Memory

- memory change: 1.06x