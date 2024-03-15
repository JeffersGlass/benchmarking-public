
# Results vs. 3.10.4

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: linux-x86_64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.36x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.29x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 263 ms: 1.32x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.97 ms: 1.39x faster                                                  |
| docutils       | 3.30 sec                                               | 2.61 sec: 1.26x faster                                                 |
| tornado_http   | 136 ms                                                 | 94.5 ms: 1.44x faster                                                  |
| Geometric mean | (ref)                                                  | 1.35x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 434 ms: 1.68x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 559 ms: 1.56x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 704 ms: 1.44x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.54x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 88.9 ms: 1.73x faster                                                  |
| float          | 117 ms                                                 | 79.4 ms: 1.47x faster                                                  |
| pidigits       | 191 ms                                                 | 195 ms: 1.02x slower                                                   |
| Geometric mean | (ref)                                                  | 1.36x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 129 ms: 1.46x faster                                                   |
| regex_v8       | 27.8 ms                                                | 25.3 ms: 1.10x faster                                                  |
| regex_dna      | 227 ms                                                 | 224 ms: 1.01x faster                                                   |
| regex_effbot   | 3.63 ms                                                | 3.77 ms: 1.04x slower                                                  |
| Geometric mean | (ref)                                                  | 1.12x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 300 us: 1.62x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 213 us: 1.55x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.11 sec: 1.49x faster                                                 |
| xml_etree_process    | 79.1 ms                                                | 58.5 ms: 1.35x faster                                                  |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 84.9 ms: 1.17x faster                                                  |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 104 ms: 1.11x faster                                                   |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.08x faster                                                   |
| pickle_list          | 5.08 us                                                | 4.92 us: 1.03x faster                                                  |
| unpickle_list        | 5.20 us                                                | 5.13 us: 1.01x faster                                                  |
| unpickle             | 14.4 us                                                | 15.0 us: 1.04x slower                                                  |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                                  |
| pickle_dict          | 29.6 us                                                | 33.4 us: 1.13x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.17x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.70 ms: 1.47x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.1 ms: 1.47x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 112 us: 4.88x faster                                                   |
| generators               | 80.1 ms                                                | 29.6 ms: 2.70x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.23 ms: 2.45x faster                                                  |
| chaos                    | 115 ms                                                 | 59.2 ms: 1.95x faster                                                  |
| raytrace                 | 507 ms                                                 | 260 ms: 1.95x faster                                                   |
| asyncio_tcp              | 922 ms                                                 | 484 ms: 1.90x faster                                                   |
| logging_silent           | 190 ns                                                 | 101 ns: 1.87x faster                                                   |
| comprehensions           | 28.8 us                                                | 16.0 us: 1.80x faster                                                  |
| crypto_pyaes             | 128 ms                                                 | 71.3 ms: 1.79x faster                                                  |
| richards_super           | 94.7 ms                                                | 53.8 ms: 1.76x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.24 ms: 1.76x faster                                                  |
| go                       | 240 ms                                                 | 138 ms: 1.73x faster                                                   |
| scimark_monte_carlo      | 118 ms                                                 | 68.3 ms: 1.73x faster                                                  |
| nbody                    | 154 ms                                                 | 88.9 ms: 1.73x faster                                                  |
| scimark_sor              | 220 ms                                                 | 129 ms: 1.71x faster                                                   |
| hexiom                   | 10.4 ms                                                | 6.20 ms: 1.68x faster                                                  |
| async_tree_none          | 728 ms                                                 | 434 ms: 1.68x faster                                                   |
| richards                 | 79.3 ms                                                | 47.4 ms: 1.67x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.57 ms: 1.64x faster                                                  |
| coroutines               | 35.1 ms                                                | 21.6 ms: 1.62x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 300 us: 1.62x faster                                                   |
| scimark_lu               | 176 ms                                                 | 111 ms: 1.59x faster                                                   |
| async_tree_memoization   | 870 ms                                                 | 559 ms: 1.56x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 213 us: 1.55x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 37.9 us: 1.54x faster                                                  |
| pyflate                  | 716 ms                                                 | 464 ms: 1.54x faster                                                   |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                 |
| spectral_norm            | 170 ms                                                 | 114 ms: 1.49x faster                                                   |
| tomli_loads              | 3.14 sec                                               | 2.11 sec: 1.49x faster                                                 |
| logging_simple           | 8.30 us                                                | 5.60 us: 1.48x faster                                                  |
| unpack_sequence          | 60.0 ns                                                | 40.5 ns: 1.48x faster                                                  |
| float                    | 117 ms                                                 | 79.4 ms: 1.47x faster                                                  |
| logging_format           | 9.09 us                                                | 6.18 us: 1.47x faster                                                  |
| mako                     | 16.3 ms                                                | 11.1 ms: 1.47x faster                                                  |
| regex_compile            | 188 ms                                                 | 129 ms: 1.46x faster                                                   |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 704 ms: 1.44x faster                                                   |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.44x faster                                                 |
| tornado_http             | 136 ms                                                 | 94.5 ms: 1.44x faster                                                  |
| pprint_pformat           | 2.10 sec                                               | 1.49 sec: 1.41x faster                                                 |
| pprint_safe_repr         | 1.02 sec                                               | 728 ms: 1.40x faster                                                   |
| deepcopy                 | 479 us                                                 | 345 us: 1.39x faster                                                   |
| chameleon                | 9.68 ms                                                | 6.97 ms: 1.39x faster                                                  |
| deepcopy_reduce          | 4.17 us                                                | 3.05 us: 1.37x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 58.5 ms: 1.35x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 106 ms: 1.35x faster                                                   |
| fannkuch                 | 532 ms                                                 | 400 ms: 1.33x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.33x faster                                                  |
| sympy_sum                | 196 ms                                                 | 148 ms: 1.33x faster                                                   |
| 2to3                     | 348 ms                                                 | 263 ms: 1.32x faster                                                   |
| scimark_fft              | 466 ms                                                 | 352 ms: 1.32x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.20 sec: 1.31x faster                                                 |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.93 ms: 1.31x faster                                                  |
| sqlglot_optimize         | 69.2 ms                                                | 53.4 ms: 1.30x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 65.4 ms: 1.29x faster                                                  |
| sympy_str                | 346 ms                                                 | 269 ms: 1.28x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.61 sec: 1.26x faster                                                 |
| nqueens                  | 106 ms                                                 | 83.9 ms: 1.26x faster                                                  |
| sympy_expand             | 566 ms                                                 | 457 ms: 1.24x faster                                                   |
| dask                     | 441 ms                                                 | 360 ms: 1.23x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 828 us: 1.19x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 84.9 ms: 1.17x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.53 sec: 1.13x faster                                                 |
| meteor_contest           | 120 ms                                                 | 107 ms: 1.11x faster                                                   |
| json_loads               | 31.2 us                                                | 28.1 us: 1.11x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 104 ms: 1.11x faster                                                   |
| pathlib                  | 20.5 ms                                                | 18.5 ms: 1.11x faster                                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 25.3 ms: 1.10x faster                                                  |
| json                     | 5.69 ms                                                | 5.21 ms: 1.09x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 156 ms: 1.08x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.82 us: 1.07x faster                                                  |
| pickle_list              | 5.08 us                                                | 4.92 us: 1.03x faster                                                  |
| unpickle_list            | 5.20 us                                                | 5.13 us: 1.01x faster                                                  |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                   |
| regex_dna                | 227 ms                                                 | 224 ms: 1.01x faster                                                   |
| async_generators         | 444 ms                                                 | 438 ms: 1.01x faster                                                   |
| pidigits                 | 191 ms                                                 | 195 ms: 1.02x slower                                                   |
| gc_traversal             | 3.62 ms                                                | 3.72 ms: 1.03x slower                                                  |
| regex_effbot             | 3.63 ms                                                | 3.77 ms: 1.04x slower                                                  |
| unpickle                 | 14.4 us                                                | 15.0 us: 1.04x slower                                                  |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                                  |
| pickle_dict              | 29.6 us                                                | 33.4 us: 1.13x slower                                                  |
| telco                    | 7.27 ms                                                | 8.32 ms: 1.15x slower                                                  |
| coverage                 | 79.4 ms                                                | 96.2 ms: 1.21x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.70 ms: 1.47x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.36x faster                                                           |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.31x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.29x


# Memory

- memory change: 1.06x