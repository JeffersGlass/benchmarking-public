# Results vs. 3.10.4

- fork: python
- ref: e7ba6e9dbe5433b4a0bc
- machine: linux-x86_64
- commit hash: e7ba6e9
- commit date: 2024-03-05
- overall geometric mean: 1.31x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: 1.34x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 276 ms: 1.26x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.81 ms: 1.42x faster                                                  |
| docutils       | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                 |
| tornado_http   | 136 ms                                                 | 96.9 ms: 1.41x faster                                                  |
| Geometric mean | (ref)                                                  | 1.32x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 434 ms: 1.68x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 561 ms: 1.55x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.49x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 704 ms: 1.44x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.54x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 94.5 ms: 1.63x faster                                                  |
| float          | 117 ms                                                 | 78.3 ms: 1.50x faster                                                  |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.35x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 142 ms: 1.33x faster                                                   |
| regex_v8       | 27.8 ms                                                | 25.3 ms: 1.10x faster                                                  |
| regex_dna      | 227 ms                                                 | 222 ms: 1.02x faster                                                   |
| regex_effbot   | 3.63 ms                                                | 3.69 ms: 1.02x slower                                                  |
| Geometric mean | (ref)                                                  | 1.10x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 297 us: 1.63x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.01 sec: 1.56x faster                                                 |
| unpickle_pure_python | 331 us                                                 | 236 us: 1.40x faster                                                   |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 58.7 ms: 1.35x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 86.5 ms: 1.15x faster                                                  |
| json_loads           | 31.2 us                                                | 27.4 us: 1.14x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                   |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| unpickle_list        | 5.20 us                                                | 4.91 us: 1.06x faster                                                  |
| pickle_list          | 5.08 us                                                | 4.89 us: 1.04x faster                                                  |
| unpickle             | 14.4 us                                                | 15.0 us: 1.04x slower                                                  |
| pickle               | 10.7 us                                                | 11.6 us: 1.09x slower                                                  |
| pickle_dict          | 29.6 us                                                | 33.8 us: 1.14x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.17x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 12.3 ms: 1.18x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 11.0 ms: 1.85x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.25x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.0 ms: 1.48x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 112 us: 4.85x faster                                                   |
| generators               | 80.1 ms                                                | 29.5 ms: 2.72x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.41 ms: 2.32x faster                                                  |
| logging_silent           | 190 ns                                                 | 99.5 ns: 1.91x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 486 ms: 1.90x faster                                                   |
| chaos                    | 115 ms                                                 | 63.6 ms: 1.82x faster                                                  |
| richards_super           | 94.7 ms                                                | 53.1 ms: 1.78x faster                                                  |
| raytrace                 | 507 ms                                                 | 287 ms: 1.77x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 72.6 ms: 1.76x faster                                                  |
| scimark_sor              | 220 ms                                                 | 127 ms: 1.72x faster                                                   |
| richards                 | 79.3 ms                                                | 46.0 ms: 1.72x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 69.5 ms: 1.70x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.28 ms: 1.69x faster                                                  |
| async_tree_none          | 728 ms                                                 | 434 ms: 1.68x faster                                                   |
| comprehensions           | 28.8 us                                                | 17.2 us: 1.67x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 297 us: 1.63x faster                                                   |
| nbody                    | 154 ms                                                 | 94.5 ms: 1.63x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.62 ms: 1.59x faster                                                  |
| coroutines               | 35.1 ms                                                | 22.3 ms: 1.57x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.01 sec: 1.56x faster                                                 |
| async_tree_memoization   | 870 ms                                                 | 561 ms: 1.55x faster                                                   |
| go                       | 240 ms                                                 | 155 ms: 1.54x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 38.6 us: 1.52x faster                                                  |
| spectral_norm            | 170 ms                                                 | 113 ms: 1.50x faster                                                   |
| float                    | 117 ms                                                 | 78.3 ms: 1.50x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.49x faster                                                 |
| mako                     | 16.3 ms                                                | 11.0 ms: 1.48x faster                                                  |
| logging_simple           | 8.30 us                                                | 5.62 us: 1.48x faster                                                  |
| hexiom                   | 10.4 ms                                                | 7.05 ms: 1.47x faster                                                  |
| pyflate                  | 716 ms                                                 | 489 ms: 1.46x faster                                                   |
| logging_format           | 9.09 us                                                | 6.23 us: 1.46x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 704 ms: 1.44x faster                                                   |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                 |
| chameleon                | 9.68 ms                                                | 6.81 ms: 1.42x faster                                                  |
| tornado_http             | 136 ms                                                 | 96.9 ms: 1.41x faster                                                  |
| unpickle_pure_python     | 331 us                                                 | 236 us: 1.40x faster                                                   |
| scimark_fft              | 466 ms                                                 | 335 ms: 1.39x faster                                                   |
| deepcopy                 | 479 us                                                 | 346 us: 1.38x faster                                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.68 ms: 1.38x faster                                                  |
| scimark_lu               | 176 ms                                                 | 128 ms: 1.38x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.04 us: 1.37x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                  |
| pprint_safe_repr         | 1.02 sec                                               | 746 ms: 1.36x faster                                                   |
| pprint_pformat           | 2.10 sec                                               | 1.54 sec: 1.36x faster                                                 |
| fannkuch                 | 532 ms                                                 | 394 ms: 1.35x faster                                                   |
| xml_etree_process        | 79.1 ms                                                | 58.7 ms: 1.35x faster                                                  |
| pycparser                | 1.58 sec                                               | 1.17 sec: 1.35x faster                                                 |
| sqlglot_normalize        | 143 ms                                                 | 107 ms: 1.34x faster                                                   |
| regex_compile            | 188 ms                                                 | 142 ms: 1.33x faster                                                   |
| 2to3                     | 348 ms                                                 | 276 ms: 1.26x faster                                                   |
| sympy_sum                | 196 ms                                                 | 157 ms: 1.25x faster                                                   |
| sqlglot_optimize         | 69.2 ms                                                | 55.7 ms: 1.24x faster                                                  |
| sympy_integrate          | 25.8 ms                                                | 20.8 ms: 1.24x faster                                                  |
| sympy_str                | 346 ms                                                 | 279 ms: 1.24x faster                                                   |
| dulwich_log              | 84.3 ms                                                | 68.4 ms: 1.23x faster                                                  |
| docutils                 | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                 |
| sympy_expand             | 566 ms                                                 | 474 ms: 1.19x faster                                                   |
| python_startup           | 14.6 ms                                                | 12.3 ms: 1.18x faster                                                  |
| nqueens                  | 106 ms                                                 | 89.6 ms: 1.18x faster                                                  |
| bench_thread_pool        | 986 us                                                 | 844 us: 1.17x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 86.5 ms: 1.15x faster                                                  |
| json_loads               | 31.2 us                                                | 27.4 us: 1.14x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                                  |
| json                     | 5.69 ms                                                | 5.12 ms: 1.11x faster                                                  |
| meteor_contest           | 120 ms                                                 | 108 ms: 1.11x faster                                                   |
| regex_v8                 | 27.8 ms                                                | 25.3 ms: 1.10x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.82 us: 1.07x faster                                                  |
| unpickle_list            | 5.20 us                                                | 4.91 us: 1.06x faster                                                  |
| pickle_list              | 5.08 us                                                | 4.89 us: 1.04x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.77 sec: 1.03x faster                                                 |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| regex_dna                | 227 ms                                                 | 222 ms: 1.02x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                   |
| regex_effbot             | 3.63 ms                                                | 3.69 ms: 1.02x slower                                                  |
| unpickle                 | 14.4 us                                                | 15.0 us: 1.04x slower                                                  |
| async_generators         | 444 ms                                                 | 468 ms: 1.05x slower                                                   |
| pickle                   | 10.7 us                                                | 11.6 us: 1.09x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 4.04 ms: 1.11x slower                                                  |
| telco                    | 7.27 ms                                                | 8.24 ms: 1.13x slower                                                  |
| pickle_dict              | 29.6 us                                                | 33.8 us: 1.14x slower                                                  |
| bench_mp_pool            | 24.0 ms                                                | 28.0 ms: 1.17x slower                                                  |
| coverage                 | 79.4 ms                                                | 95.4 ms: 1.20x slower                                                  |
| dask                     | 441 ms                                                 | 530 ms: 1.20x slower                                                   |
| unpack_sequence          | 60.0 ns                                                | 86.3 ns: 1.44x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 11.0 ms: 1.85x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.31x faster                                                           |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240305-3.13.0a4+-e7ba6e9-JIT/bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.25x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: 1.34x