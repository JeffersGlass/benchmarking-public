
# Results vs. 3.10.4

- fork: mdboom
- ref: force_malloc
- machine: linux-x86_64
- commit hash: 0320909
- commit date: 2024-02-14
- overall geometric mean: 1.37x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.30x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 262 ms: 1.33x faster                                           |
| chameleon      | 9.68 ms                                                | 6.82 ms: 1.42x faster                                          |
| docutils       | 3.30 sec                                               | 2.59 sec: 1.27x faster                                         |
| tornado_http   | 136 ms                                                 | 94.8 ms: 1.44x faster                                          |
| Geometric mean | (ref)                                                  | 1.37x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 424 ms: 1.72x faster                                           |
| async_tree_memoization  | 870 ms                                                 | 553 ms: 1.57x faster                                           |
| async_tree_io           | 1.77 sec                                               | 1.15 sec: 1.54x faster                                         |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 697 ms: 1.46x faster                                           |
| Geometric mean          | (ref)                                                  | 1.57x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 91.9 ms: 1.67x faster                                          |
| float          | 117 ms                                                 | 76.2 ms: 1.54x faster                                          |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                           |
| Geometric mean | (ref)                                                  | 1.38x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 127 ms: 1.48x faster                                           |
| regex_v8       | 27.8 ms                                                | 25.2 ms: 1.10x faster                                          |
| regex_dna      | 227 ms                                                 | 220 ms: 1.03x faster                                           |
| Geometric mean | (ref)                                                  | 1.14x faster                                                   |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 291 us: 1.66x faster                                           |
| unpickle_pure_python | 331 us                                                 | 212 us: 1.56x faster                                           |
| tomli_loads          | 3.14 sec                                               | 2.13 sec: 1.48x faster                                         |
| xml_etree_process    | 79.1 ms                                                | 57.9 ms: 1.37x faster                                          |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                          |
| xml_etree_generate   | 99.4 ms                                                | 84.5 ms: 1.18x faster                                          |
| json_loads           | 31.2 us                                                | 27.7 us: 1.13x faster                                          |
| xml_etree_iterparse  | 115 ms                                                 | 104 ms: 1.11x faster                                           |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.08x faster                                           |
| unpickle_list        | 5.20 us                                                | 4.89 us: 1.06x faster                                          |
| pickle_list          | 5.08 us                                                | 5.13 us: 1.01x slower                                          |
| unpickle             | 14.4 us                                                | 15.4 us: 1.07x slower                                          |
| pickle               | 10.7 us                                                | 11.8 us: 1.10x slower                                          |
| pickle_dict          | 29.6 us                                                | 34.7 us: 1.17x slower                                          |
| Geometric mean       | (ref)                                                  | 1.17x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.45x faster                                          |
| python_startup_no_site | 5.93 ms                                                | 8.70 ms: 1.47x slower                                          |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.1 ms: 1.47x faster                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 108 us: 5.06x faster                                           |
| generators               | 80.1 ms                                                | 29.5 ms: 2.71x faster                                          |
| deltablue                | 7.91 ms                                                | 3.16 ms: 2.50x faster                                          |
| logging_silent           | 190 ns                                                 | 95.2 ns: 1.99x faster                                          |
| raytrace                 | 507 ms                                                 | 258 ms: 1.97x faster                                           |
| chaos                    | 115 ms                                                 | 59.5 ms: 1.94x faster                                          |
| asyncio_tcp              | 922 ms                                                 | 484 ms: 1.90x faster                                           |
| scimark_sor              | 220 ms                                                 | 117 ms: 1.87x faster                                           |
| crypto_pyaes             | 128 ms                                                 | 70.6 ms: 1.81x faster                                          |
| comprehensions           | 28.8 us                                                | 15.9 us: 1.81x faster                                          |
| richards_super           | 94.7 ms                                                | 52.7 ms: 1.80x faster                                          |
| scimark_monte_carlo      | 118 ms                                                 | 66.3 ms: 1.78x faster                                          |
| go                       | 240 ms                                                 | 135 ms: 1.77x faster                                           |
| sqlglot_parse            | 2.17 ms                                                | 1.25 ms: 1.74x faster                                          |
| hexiom                   | 10.4 ms                                                | 6.04 ms: 1.72x faster                                          |
| async_tree_none          | 728 ms                                                 | 424 ms: 1.72x faster                                           |
| richards                 | 79.3 ms                                                | 47.0 ms: 1.69x faster                                          |
| nbody                    | 154 ms                                                 | 91.9 ms: 1.67x faster                                          |
| pickle_pure_python       | 484 us                                                 | 291 us: 1.66x faster                                           |
| sqlglot_transpile        | 2.57 ms                                                | 1.56 ms: 1.65x faster                                          |
| coroutines               | 35.1 ms                                                | 21.5 ms: 1.63x faster                                          |
| pyflate                  | 716 ms                                                 | 447 ms: 1.60x faster                                           |
| scimark_lu               | 176 ms                                                 | 111 ms: 1.59x faster                                           |
| deepcopy_memo            | 58.5 us                                                | 37.1 us: 1.57x faster                                          |
| async_tree_memoization   | 870 ms                                                 | 553 ms: 1.57x faster                                           |
| spectral_norm            | 170 ms                                                 | 108 ms: 1.57x faster                                           |
| unpickle_pure_python     | 331 us                                                 | 212 us: 1.56x faster                                           |
| async_tree_io            | 1.77 sec                                               | 1.15 sec: 1.54x faster                                         |
| float                    | 117 ms                                                 | 76.2 ms: 1.54x faster                                          |
| logging_simple           | 8.30 us                                                | 5.56 us: 1.49x faster                                          |
| logging_format           | 9.09 us                                                | 6.09 us: 1.49x faster                                          |
| regex_compile            | 188 ms                                                 | 127 ms: 1.48x faster                                           |
| tomli_loads              | 3.14 sec                                               | 2.13 sec: 1.48x faster                                         |
| mako                     | 16.3 ms                                                | 11.1 ms: 1.47x faster                                          |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 697 ms: 1.46x faster                                           |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.45x faster                                          |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.44x faster                                         |
| tornado_http             | 136 ms                                                 | 94.8 ms: 1.44x faster                                          |
| chameleon                | 9.68 ms                                                | 6.82 ms: 1.42x faster                                          |
| deepcopy                 | 479 us                                                 | 338 us: 1.42x faster                                           |
| deepcopy_reduce          | 4.17 us                                                | 2.95 us: 1.41x faster                                          |
| pprint_pformat           | 2.10 sec                                               | 1.49 sec: 1.41x faster                                         |
| fannkuch                 | 532 ms                                                 | 381 ms: 1.40x faster                                           |
| pprint_safe_repr         | 1.02 sec                                               | 732 ms: 1.39x faster                                           |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.66 ms: 1.39x faster                                          |
| xml_etree_process        | 79.1 ms                                                | 57.9 ms: 1.37x faster                                          |
| pycparser                | 1.58 sec                                               | 1.16 sec: 1.36x faster                                         |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                          |
| sqlglot_normalize        | 143 ms                                                 | 105 ms: 1.36x faster                                           |
| 2to3                     | 348 ms                                                 | 262 ms: 1.33x faster                                           |
| sympy_integrate          | 25.8 ms                                                | 19.4 ms: 1.33x faster                                          |
| sympy_sum                | 196 ms                                                 | 148 ms: 1.33x faster                                           |
| scimark_fft              | 466 ms                                                 | 354 ms: 1.32x faster                                           |
| nqueens                  | 106 ms                                                 | 80.6 ms: 1.31x faster                                          |
| sympy_str                | 346 ms                                                 | 266 ms: 1.30x faster                                           |
| sqlglot_optimize         | 69.2 ms                                                | 53.2 ms: 1.30x faster                                          |
| dulwich_log              | 84.3 ms                                                | 65.2 ms: 1.29x faster                                          |
| docutils                 | 3.30 sec                                               | 2.59 sec: 1.27x faster                                         |
| sympy_expand             | 566 ms                                                 | 451 ms: 1.25x faster                                           |
| bench_thread_pool        | 986 us                                                 | 798 us: 1.24x faster                                           |
| dask                     | 441 ms                                                 | 360 ms: 1.23x faster                                           |
| unpack_sequence          | 60.0 ns                                                | 49.8 ns: 1.21x faster                                          |
| xml_etree_generate       | 99.4 ms                                                | 84.5 ms: 1.18x faster                                          |
| mdp                      | 2.85 sec                                               | 2.51 sec: 1.14x faster                                         |
| pathlib                  | 20.5 ms                                                | 18.0 ms: 1.13x faster                                          |
| json_loads               | 31.2 us                                                | 27.7 us: 1.13x faster                                          |
| json                     | 5.69 ms                                                | 5.08 ms: 1.12x faster                                          |
| meteor_contest           | 120 ms                                                 | 107 ms: 1.12x faster                                           |
| create_gc_cycles         | 1.62 ms                                                | 1.46 ms: 1.11x faster                                          |
| xml_etree_iterparse      | 115 ms                                                 | 104 ms: 1.11x faster                                           |
| regex_v8                 | 27.8 ms                                                | 25.2 ms: 1.10x faster                                          |
| xml_etree_parse          | 168 ms                                                 | 156 ms: 1.08x faster                                           |
| sqlite_synth             | 3.02 us                                                | 2.80 us: 1.08x faster                                          |
| unpickle_list            | 5.20 us                                                | 4.89 us: 1.06x faster                                          |
| regex_dna                | 227 ms                                                 | 220 ms: 1.03x faster                                           |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                           |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                           |
| async_generators         | 444 ms                                                 | 442 ms: 1.00x faster                                           |
| pickle_list              | 5.08 us                                                | 5.13 us: 1.01x slower                                          |
| gc_traversal             | 3.62 ms                                                | 3.69 ms: 1.02x slower                                          |
| unpickle                 | 14.4 us                                                | 15.4 us: 1.07x slower                                          |
| pickle                   | 10.7 us                                                | 11.8 us: 1.10x slower                                          |
| telco                    | 7.27 ms                                                | 8.35 ms: 1.15x slower                                          |
| pickle_dict              | 29.6 us                                                | 34.7 us: 1.17x slower                                          |
| coverage                 | 79.4 ms                                                | 95.9 ms: 1.21x slower                                          |
| python_startup_no_site   | 5.93 ms                                                | 8.70 ms: 1.47x slower                                          |
| Geometric mean           | (ref)                                                  | 1.37x faster                                                   |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240214-3.13.0a3+-0320909/bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.33x
- 95% likely to have a speedup of 1.31x
- 99% likely to have a speedup of 1.30x


# Memory

- memory change: 1.07x