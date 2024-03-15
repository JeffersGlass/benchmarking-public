
# Results vs. 3.10.4

- fork: brandtbucher
- ref: counter_table
- machine: linux-x86_64
- commit hash: c49f898
- commit date: 2024-01-04
- overall geometric mean: 1.35x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.28x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 266 ms: 1.31x faster                                                  |
| chameleon      | 9.68 ms                                                | 6.96 ms: 1.39x faster                                                 |
| docutils       | 3.30 sec                                               | 2.62 sec: 1.26x faster                                                |
| tornado_http   | 136 ms                                                 | 94.9 ms: 1.44x faster                                                 |
| Geometric mean | (ref)                                                  | 1.35x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 436 ms: 1.67x faster                                                  |
| async_tree_memoization  | 870 ms                                                 | 562 ms: 1.55x faster                                                  |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 707 ms: 1.44x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.54x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 88.9 ms: 1.73x faster                                                 |
| float          | 117 ms                                                 | 80.2 ms: 1.46x faster                                                 |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                  |
| Geometric mean | (ref)                                                  | 1.37x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 131 ms: 1.44x faster                                                  |
| regex_v8       | 27.8 ms                                                | 25.4 ms: 1.09x faster                                                 |
| regex_dna      | 227 ms                                                 | 217 ms: 1.04x faster                                                  |
| Geometric mean | (ref)                                                  | 1.13x faster                                                          |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 295 us: 1.64x faster                                                  |
| unpickle_pure_python | 331 us                                                 | 218 us: 1.52x faster                                                  |
| tomli_loads          | 3.14 sec                                               | 2.13 sec: 1.47x faster                                                |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                 |
| xml_etree_process    | 79.1 ms                                                | 60.1 ms: 1.32x faster                                                 |
| xml_etree_generate   | 99.4 ms                                                | 87.2 ms: 1.14x faster                                                 |
| json_loads           | 31.2 us                                                | 28.2 us: 1.11x faster                                                 |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                  |
| pickle_list          | 5.08 us                                                | 4.87 us: 1.04x faster                                                 |
| unpickle_list        | 5.20 us                                                | 5.29 us: 1.02x slower                                                 |
| pickle               | 10.7 us                                                | 11.3 us: 1.06x slower                                                 |
| unpickle             | 14.4 us                                                | 15.8 us: 1.10x slower                                                 |
| pickle_dict          | 29.6 us                                                | 34.9 us: 1.18x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                 |
| python_startup_no_site | 5.93 ms                                                | 8.82 ms: 1.49x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 10.9 ms: 1.49x faster                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 112 us: 4.88x faster                                                  |
| generators               | 80.1 ms                                                | 29.7 ms: 2.70x faster                                                 |
| deltablue                | 7.91 ms                                                | 3.24 ms: 2.44x faster                                                 |
| chaos                    | 115 ms                                                 | 58.8 ms: 1.96x faster                                                 |
| raytrace                 | 507 ms                                                 | 261 ms: 1.94x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 488 ms: 1.89x faster                                                  |
| scimark_sor              | 220 ms                                                 | 121 ms: 1.82x faster                                                  |
| logging_silent           | 190 ns                                                 | 104 ns: 1.82x faster                                                  |
| crypto_pyaes             | 128 ms                                                 | 71.5 ms: 1.79x faster                                                 |
| scimark_monte_carlo      | 118 ms                                                 | 66.9 ms: 1.77x faster                                                 |
| go                       | 240 ms                                                 | 138 ms: 1.74x faster                                                  |
| comprehensions           | 28.8 us                                                | 16.6 us: 1.74x faster                                                 |
| sqlglot_parse            | 2.17 ms                                                | 1.25 ms: 1.73x faster                                                 |
| nbody                    | 154 ms                                                 | 88.9 ms: 1.73x faster                                                 |
| richards_super           | 94.7 ms                                                | 55.1 ms: 1.72x faster                                                 |
| async_tree_none          | 728 ms                                                 | 436 ms: 1.67x faster                                                  |
| hexiom                   | 10.4 ms                                                | 6.27 ms: 1.66x faster                                                 |
| pickle_pure_python       | 484 us                                                 | 295 us: 1.64x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.58 ms: 1.63x faster                                                 |
| coroutines               | 35.1 ms                                                | 21.5 ms: 1.63x faster                                                 |
| richards                 | 79.3 ms                                                | 49.1 ms: 1.62x faster                                                 |
| spectral_norm            | 170 ms                                                 | 110 ms: 1.55x faster                                                  |
| async_tree_memoization   | 870 ms                                                 | 562 ms: 1.55x faster                                                  |
| pyflate                  | 716 ms                                                 | 464 ms: 1.54x faster                                                  |
| scimark_lu               | 176 ms                                                 | 116 ms: 1.52x faster                                                  |
| unpickle_pure_python     | 331 us                                                 | 218 us: 1.52x faster                                                  |
| deepcopy_memo            | 58.5 us                                                | 38.6 us: 1.52x faster                                                 |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                |
| mako                     | 16.3 ms                                                | 10.9 ms: 1.49x faster                                                 |
| tomli_loads              | 3.14 sec                                               | 2.13 sec: 1.47x faster                                                |
| logging_simple           | 8.30 us                                                | 5.64 us: 1.47x faster                                                 |
| float                    | 117 ms                                                 | 80.2 ms: 1.46x faster                                                 |
| logging_format           | 9.09 us                                                | 6.24 us: 1.46x faster                                                 |
| regex_compile            | 188 ms                                                 | 131 ms: 1.44x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.44x faster                                                |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 707 ms: 1.44x faster                                                  |
| tornado_http             | 136 ms                                                 | 94.9 ms: 1.44x faster                                                 |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                 |
| pprint_pformat           | 2.10 sec                                               | 1.50 sec: 1.40x faster                                                |
| chameleon                | 9.68 ms                                                | 6.96 ms: 1.39x faster                                                 |
| pprint_safe_repr         | 1.02 sec                                               | 739 ms: 1.38x faster                                                  |
| deepcopy                 | 479 us                                                 | 350 us: 1.37x faster                                                  |
| fannkuch                 | 532 ms                                                 | 392 ms: 1.36x faster                                                  |
| deepcopy_reduce          | 4.17 us                                                | 3.09 us: 1.35x faster                                                 |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                 |
| sqlglot_normalize        | 143 ms                                                 | 107 ms: 1.34x faster                                                  |
| sympy_sum                | 196 ms                                                 | 149 ms: 1.32x faster                                                  |
| pycparser                | 1.58 sec                                               | 1.19 sec: 1.32x faster                                                |
| xml_etree_process        | 79.1 ms                                                | 60.1 ms: 1.32x faster                                                 |
| 2to3                     | 348 ms                                                 | 266 ms: 1.31x faster                                                  |
| sympy_integrate          | 25.8 ms                                                | 19.8 ms: 1.31x faster                                                 |
| scimark_fft              | 466 ms                                                 | 357 ms: 1.30x faster                                                  |
| sympy_str                | 346 ms                                                 | 270 ms: 1.28x faster                                                  |
| sqlglot_optimize         | 69.2 ms                                                | 54.1 ms: 1.28x faster                                                 |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.07 ms: 1.28x faster                                                 |
| nqueens                  | 106 ms                                                 | 83.1 ms: 1.27x faster                                                 |
| dulwich_log              | 84.3 ms                                                | 66.2 ms: 1.27x faster                                                 |
| docutils                 | 3.30 sec                                               | 2.62 sec: 1.26x faster                                                |
| sympy_expand             | 566 ms                                                 | 456 ms: 1.24x faster                                                  |
| dask                     | 441 ms                                                 | 362 ms: 1.22x faster                                                  |
| unpack_sequence          | 60.0 ns                                                | 49.7 ns: 1.21x faster                                                 |
| bench_thread_pool        | 986 us                                                 | 838 us: 1.18x faster                                                  |
| xml_etree_generate       | 99.4 ms                                                | 87.2 ms: 1.14x faster                                                 |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                                 |
| json_loads               | 31.2 us                                                | 28.2 us: 1.11x faster                                                 |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.11x faster                                                 |
| regex_v8                 | 27.8 ms                                                | 25.4 ms: 1.09x faster                                                 |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                  |
| json                     | 5.69 ms                                                | 5.23 ms: 1.09x faster                                                 |
| meteor_contest           | 120 ms                                                 | 110 ms: 1.09x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                  |
| sqlite_synth             | 3.02 us                                                | 2.85 us: 1.06x faster                                                 |
| regex_dna                | 227 ms                                                 | 217 ms: 1.04x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.73 sec: 1.04x faster                                                |
| pickle_list              | 5.08 us                                                | 4.87 us: 1.04x faster                                                 |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                  |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                  |
| gc_traversal             | 3.62 ms                                                | 3.60 ms: 1.01x faster                                                 |
| async_generators         | 444 ms                                                 | 450 ms: 1.01x slower                                                  |
| unpickle_list            | 5.20 us                                                | 5.29 us: 1.02x slower                                                 |
| pickle                   | 10.7 us                                                | 11.3 us: 1.06x slower                                                 |
| unpickle                 | 14.4 us                                                | 15.8 us: 1.10x slower                                                 |
| telco                    | 7.27 ms                                                | 8.21 ms: 1.13x slower                                                 |
| pickle_dict              | 29.6 us                                                | 34.9 us: 1.18x slower                                                 |
| coverage                 | 79.4 ms                                                | 95.4 ms: 1.20x slower                                                 |
| python_startup_no_site   | 5.93 ms                                                | 8.82 ms: 1.49x slower                                                 |
| Geometric mean           | (ref)                                                  | 1.35x faster                                                          |

Benchmark hidden because not significant (3): mypy2, regex_effbot, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240104-3.13.0a2+-c49f898/bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.30x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.28x


# Memory

- memory change: 1.06x