# Results vs. 3.12.0

- fork: python
- ref: e7ba6e9dbe5433b4a0bc
- machine: linux-x86_64
- commit hash: e7ba6e9
- commit date: 2024-03-05
- overall geometric mean: 1.01x faster \*
- HPT reliability: 98.67%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 276 ms: 1.01x slower                                                   |
| chameleon      | 7.41 ms                                                | 6.81 ms: 1.09x faster                                                  |
| docutils       | 2.77 sec                                               | 2.70 sec: 1.02x faster                                                 |
| tornado_http   | 103 ms                                                 | 96.9 ms: 1.06x faster                                                  |
| Geometric mean | (ref)                                                  | 1.04x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 434 ms: 1.09x faster                                                   |
| async_tree_cpu_io_mixed | 726 ms                                                 | 704 ms: 1.03x faster                                                   |
| async_tree_memoization  | 578 ms                                                 | 561 ms: 1.03x faster                                                   |
| async_tree_none_tg      | 450 ms                                                 | 446 ms: 1.01x faster                                                   |
| async_tree_io_tg        | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| async_tree_io           | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (2): async_tree_memoization_tg, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 78.3 ms: 1.08x faster                                                  |
| nbody          | 97.0 ms                                                | 94.5 ms: 1.03x faster                                                  |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                                   |
| Geometric mean | (ref)                                                  | 1.04x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 142 ms: 1.04x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.69 ms: 1.02x slower                                                  |
| regex_dna      | 212 ms                                                 | 222 ms: 1.05x slower                                                   |
| regex_v8       | 23.1 ms                                                | 25.3 ms: 1.09x slower                                                  |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.01 sec: 1.16x faster                                                 |
| pickle_pure_python   | 324 us                                                 | 297 us: 1.09x faster                                                   |
| unpickle_list        | 5.29 us                                                | 4.91 us: 1.08x faster                                                  |
| unpickle             | 15.9 us                                                | 15.0 us: 1.06x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 58.7 ms: 1.05x faster                                                  |
| pickle_dict          | 35.5 us                                                | 33.8 us: 1.05x faster                                                  |
| json_loads           | 28.5 us                                                | 27.4 us: 1.04x faster                                                  |
| pickle_list          | 5.08 us                                                | 4.89 us: 1.04x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 86.5 ms: 1.03x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.02x faster                                                   |
| xml_etree_iterparse  | 107 ms                                                 | 106 ms: 1.01x faster                                                   |
| unpickle_pure_python | 230 us                                                 | 236 us: 1.02x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                           |

Benchmark hidden because not significant (2): json_dumps, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.3 ms: 1.29x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 11.0 ms: 1.58x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.43x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.0 ms: 1.08x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 112 us: 1.41x faster                                                   |
| comprehensions           | 21.8 us                                                | 17.2 us: 1.27x faster                                                  |
| logging_format           | 7.23 us                                                | 6.23 us: 1.16x faster                                                  |
| tomli_loads              | 2.33 sec                                               | 2.01 sec: 1.16x faster                                                 |
| logging_simple           | 6.46 us                                                | 5.62 us: 1.15x faster                                                  |
| scimark_fft              | 382 ms                                                 | 335 ms: 1.14x faster                                                   |
| crypto_pyaes             | 81.9 ms                                                | 72.6 ms: 1.13x faster                                                  |
| deepcopy_reduce          | 3.35 us                                                | 3.04 us: 1.10x faster                                                  |
| pickle_pure_python       | 324 us                                                 | 297 us: 1.09x faster                                                   |
| raytrace                 | 312 ms                                                 | 287 ms: 1.09x faster                                                   |
| deltablue                | 3.72 ms                                                | 3.41 ms: 1.09x faster                                                  |
| chameleon                | 7.41 ms                                                | 6.81 ms: 1.09x faster                                                  |
| async_tree_none          | 472 ms                                                 | 434 ms: 1.09x faster                                                   |
| float                    | 84.7 ms                                                | 78.3 ms: 1.08x faster                                                  |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.68 ms: 1.08x faster                                                  |
| scimark_monte_carlo      | 75.1 ms                                                | 69.5 ms: 1.08x faster                                                  |
| sympy_sum                | 169 ms                                                 | 157 ms: 1.08x faster                                                   |
| unpickle_list            | 5.29 us                                                | 4.91 us: 1.08x faster                                                  |
| mako                     | 11.9 ms                                                | 11.0 ms: 1.08x faster                                                  |
| sympy_str                | 300 ms                                                 | 279 ms: 1.07x faster                                                   |
| deepcopy                 | 371 us                                                 | 346 us: 1.07x faster                                                   |
| sqlglot_parse            | 1.36 ms                                                | 1.28 ms: 1.06x faster                                                  |
| unpickle                 | 15.9 us                                                | 15.0 us: 1.06x faster                                                  |
| generators               | 31.2 ms                                                | 29.5 ms: 1.06x faster                                                  |
| tornado_http             | 103 ms                                                 | 96.9 ms: 1.06x faster                                                  |
| fannkuch                 | 417 ms                                                 | 394 ms: 1.06x faster                                                   |
| deepcopy_memo            | 40.7 us                                                | 38.6 us: 1.06x faster                                                  |
| chaos                    | 67.0 ms                                                | 63.6 ms: 1.05x faster                                                  |
| pathlib                  | 19.3 ms                                                | 18.4 ms: 1.05x faster                                                  |
| xml_etree_process        | 61.7 ms                                                | 58.7 ms: 1.05x faster                                                  |
| pickle_dict              | 35.5 us                                                | 33.8 us: 1.05x faster                                                  |
| logging_silent           | 104 ns                                                 | 99.5 ns: 1.05x faster                                                  |
| regex_compile            | 148 ms                                                 | 142 ms: 1.04x faster                                                   |
| sqlglot_transpile        | 1.68 ms                                                | 1.62 ms: 1.04x faster                                                  |
| pprint_safe_repr         | 776 ms                                                 | 746 ms: 1.04x faster                                                   |
| meteor_contest           | 112 ms                                                 | 108 ms: 1.04x faster                                                   |
| json_loads               | 28.5 us                                                | 27.4 us: 1.04x faster                                                  |
| pickle_list              | 5.08 us                                                | 4.89 us: 1.04x faster                                                  |
| coroutines               | 23.2 ms                                                | 22.3 ms: 1.04x faster                                                  |
| sqlglot_normalize        | 110 ms                                                 | 107 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 704 ms: 1.03x faster                                                   |
| xml_etree_generate       | 89.2 ms                                                | 86.5 ms: 1.03x faster                                                  |
| sympy_integrate          | 21.4 ms                                                | 20.8 ms: 1.03x faster                                                  |
| async_tree_memoization   | 578 ms                                                 | 561 ms: 1.03x faster                                                   |
| json                     | 5.26 ms                                                | 5.12 ms: 1.03x faster                                                  |
| nbody                    | 97.0 ms                                                | 94.5 ms: 1.03x faster                                                  |
| docutils                 | 2.77 sec                                               | 2.70 sec: 1.02x faster                                                 |
| xml_etree_parse          | 159 ms                                                 | 157 ms: 1.02x faster                                                   |
| pprint_pformat           | 1.57 sec                                               | 1.54 sec: 1.02x faster                                                 |
| spectral_norm            | 115 ms                                                 | 113 ms: 1.02x faster                                                   |
| scimark_sor              | 129 ms                                                 | 127 ms: 1.01x faster                                                   |
| asyncio_tcp              | 491 ms                                                 | 486 ms: 1.01x faster                                                   |
| sympy_expand             | 478 ms                                                 | 474 ms: 1.01x faster                                                   |
| async_tree_none_tg       | 450 ms                                                 | 446 ms: 1.01x faster                                                   |
| pycparser                | 1.18 sec                                               | 1.17 sec: 1.01x faster                                                 |
| xml_etree_iterparse      | 107 ms                                                 | 106 ms: 1.01x faster                                                   |
| pidigits                 | 187 ms                                                 | 187 ms: 1.00x faster                                                   |
| bench_thread_pool        | 842 us                                                 | 844 us: 1.00x slower                                                   |
| 2to3                     | 274 ms                                                 | 276 ms: 1.01x slower                                                   |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                 |
| async_generators         | 463 ms                                                 | 468 ms: 1.01x slower                                                   |
| pyflate                  | 482 ms                                                 | 489 ms: 1.01x slower                                                   |
| create_gc_cycles         | 1.48 ms                                                | 1.50 ms: 1.02x slower                                                  |
| sqlglot_optimize         | 54.8 ms                                                | 55.7 ms: 1.02x slower                                                  |
| async_tree_io_tg         | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| regex_effbot             | 3.61 ms                                                | 3.69 ms: 1.02x slower                                                  |
| async_tree_io            | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                 |
| unpickle_pure_python     | 230 us                                                 | 236 us: 1.02x slower                                                   |
| richards_super           | 51.5 ms                                                | 53.1 ms: 1.03x slower                                                  |
| regex_dna                | 212 ms                                                 | 222 ms: 1.05x slower                                                   |
| mdp                      | 2.63 sec                                               | 2.77 sec: 1.05x slower                                                 |
| gc_traversal             | 3.79 ms                                                | 4.04 ms: 1.06x slower                                                  |
| nqueens                  | 83.3 ms                                                | 89.6 ms: 1.08x slower                                                  |
| scimark_lu               | 118 ms                                                 | 128 ms: 1.08x slower                                                   |
| regex_v8                 | 23.1 ms                                                | 25.3 ms: 1.09x slower                                                  |
| hexiom                   | 6.41 ms                                                | 7.05 ms: 1.10x slower                                                  |
| go                       | 139 ms                                                 | 155 ms: 1.11x slower                                                   |
| telco                    | 7.10 ms                                                | 8.24 ms: 1.16x slower                                                  |
| bench_mp_pool            | 24.0 ms                                                | 28.0 ms: 1.17x slower                                                  |
| python_startup           | 9.55 ms                                                | 12.3 ms: 1.29x slower                                                  |
| coverage                 | 72.7 ms                                                | 95.4 ms: 1.31x slower                                                  |
| dask                     | 372 ms                                                 | 530 ms: 1.43x slower                                                   |
| python_startup_no_site   | 6.94 ms                                                | 11.0 ms: 1.58x slower                                                  |
| unpack_sequence          | 54.0 ns                                                | 86.3 ns: 1.60x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (9): sqlite_synth, async_tree_memoization_tg, dulwich_log, json_dumps, async_tree_cpu_io_mixed_tg, pickle, asyncio_websockets, richards, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 98.67% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.17x