
# Results vs. 3.12.0

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: linux-x86_64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.04x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 263 ms: 1.04x faster                                                   |
| chameleon      | 7.41 ms                                                | 6.97 ms: 1.06x faster                                                  |
| docutils       | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                 |
| tornado_http   | 103 ms                                                 | 94.5 ms: 1.09x faster                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 434 ms: 1.09x faster                                                   |
| async_tree_memoization  | 578 ms                                                 | 559 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed | 726 ms                                                 | 704 ms: 1.03x faster                                                   |
| async_tree_none_tg      | 450 ms                                                 | 441 ms: 1.02x faster                                                   |
| async_tree_io_tg        | 1.18 sec                                               | 1.20 sec: 1.01x slower                                                 |
| async_tree_io           | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 88.9 ms: 1.09x faster                                                  |
| float          | 84.7 ms                                                | 79.4 ms: 1.07x faster                                                  |
| pidigits       | 187 ms                                                 | 195 ms: 1.04x slower                                                   |
| Geometric mean | (ref)                                                  | 1.04x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 129 ms: 1.15x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.77 ms: 1.04x slower                                                  |
| regex_dna      | 212 ms                                                 | 224 ms: 1.06x slower                                                   |
| regex_v8       | 23.1 ms                                                | 25.3 ms: 1.09x slower                                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.11 sec: 1.10x faster                                                 |
| pickle_pure_python   | 324 us                                                 | 300 us: 1.08x faster                                                   |
| unpickle_pure_python | 230 us                                                 | 213 us: 1.08x faster                                                   |
| pickle_dict          | 35.5 us                                                | 33.4 us: 1.06x faster                                                  |
| unpickle             | 15.9 us                                                | 15.0 us: 1.06x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 58.5 ms: 1.06x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 84.9 ms: 1.05x faster                                                  |
| pickle_list          | 5.08 us                                                | 4.92 us: 1.03x faster                                                  |
| unpickle_list        | 5.29 us                                                | 5.13 us: 1.03x faster                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 104 ms: 1.03x faster                                                   |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                                   |
| json_loads           | 28.5 us                                                | 28.1 us: 1.01x faster                                                  |
| pickle               | 11.6 us                                                | 11.5 us: 1.00x faster                                                  |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.70 ms: 1.25x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.1 ms: 1.07x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 112 us: 1.41x faster                                                   |
| comprehensions           | 21.8 us                                                | 16.0 us: 1.36x faster                                                  |
| unpack_sequence          | 54.0 ns                                                | 40.5 ns: 1.33x faster                                                  |
| raytrace                 | 312 ms                                                 | 260 ms: 1.20x faster                                                   |
| logging_format           | 7.23 us                                                | 6.18 us: 1.17x faster                                                  |
| logging_simple           | 6.46 us                                                | 5.60 us: 1.15x faster                                                  |
| regex_compile            | 148 ms                                                 | 129 ms: 1.15x faster                                                   |
| deltablue                | 3.72 ms                                                | 3.23 ms: 1.15x faster                                                  |
| crypto_pyaes             | 81.9 ms                                                | 71.3 ms: 1.15x faster                                                  |
| sympy_sum                | 169 ms                                                 | 148 ms: 1.14x faster                                                   |
| chaos                    | 67.0 ms                                                | 59.2 ms: 1.13x faster                                                  |
| sympy_str                | 300 ms                                                 | 269 ms: 1.11x faster                                                   |
| tomli_loads              | 2.33 sec                                               | 2.11 sec: 1.10x faster                                                 |
| sqlglot_parse            | 1.36 ms                                                | 1.24 ms: 1.10x faster                                                  |
| sympy_integrate          | 21.4 ms                                                | 19.5 ms: 1.10x faster                                                  |
| scimark_monte_carlo      | 75.1 ms                                                | 68.3 ms: 1.10x faster                                                  |
| deepcopy_reduce          | 3.35 us                                                | 3.05 us: 1.10x faster                                                  |
| nbody                    | 97.0 ms                                                | 88.9 ms: 1.09x faster                                                  |
| async_tree_none          | 472 ms                                                 | 434 ms: 1.09x faster                                                   |
| tornado_http             | 103 ms                                                 | 94.5 ms: 1.09x faster                                                  |
| scimark_fft              | 382 ms                                                 | 352 ms: 1.09x faster                                                   |
| pickle_pure_python       | 324 us                                                 | 300 us: 1.08x faster                                                   |
| unpickle_pure_python     | 230 us                                                 | 213 us: 1.08x faster                                                   |
| deepcopy                 | 371 us                                                 | 345 us: 1.08x faster                                                   |
| deepcopy_memo            | 40.7 us                                                | 37.9 us: 1.08x faster                                                  |
| sqlglot_transpile        | 1.68 ms                                                | 1.57 ms: 1.07x faster                                                  |
| coroutines               | 23.2 ms                                                | 21.6 ms: 1.07x faster                                                  |
| mako                     | 11.9 ms                                                | 11.1 ms: 1.07x faster                                                  |
| float                    | 84.7 ms                                                | 79.4 ms: 1.07x faster                                                  |
| scimark_lu               | 118 ms                                                 | 111 ms: 1.07x faster                                                   |
| pprint_safe_repr         | 776 ms                                                 | 728 ms: 1.07x faster                                                   |
| chameleon                | 7.41 ms                                                | 6.97 ms: 1.06x faster                                                  |
| pickle_dict              | 35.5 us                                                | 33.4 us: 1.06x faster                                                  |
| docutils                 | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                 |
| unpickle                 | 15.9 us                                                | 15.0 us: 1.06x faster                                                  |
| async_generators         | 463 ms                                                 | 438 ms: 1.06x faster                                                   |
| xml_etree_process        | 61.7 ms                                                | 58.5 ms: 1.06x faster                                                  |
| generators               | 31.2 ms                                                | 29.6 ms: 1.05x faster                                                  |
| xml_etree_generate       | 89.2 ms                                                | 84.9 ms: 1.05x faster                                                  |
| pprint_pformat           | 1.57 sec                                               | 1.49 sec: 1.05x faster                                                 |
| pathlib                  | 19.3 ms                                                | 18.5 ms: 1.05x faster                                                  |
| sympy_expand             | 478 ms                                                 | 457 ms: 1.05x faster                                                   |
| dulwich_log              | 68.5 ms                                                | 65.4 ms: 1.05x faster                                                  |
| meteor_contest           | 112 ms                                                 | 107 ms: 1.05x faster                                                   |
| fannkuch                 | 417 ms                                                 | 400 ms: 1.04x faster                                                   |
| 2to3                     | 274 ms                                                 | 263 ms: 1.04x faster                                                   |
| mdp                      | 2.63 sec                                               | 2.53 sec: 1.04x faster                                                 |
| sqlglot_normalize        | 110 ms                                                 | 106 ms: 1.04x faster                                                   |
| pyflate                  | 482 ms                                                 | 464 ms: 1.04x faster                                                   |
| hexiom                   | 6.41 ms                                                | 6.20 ms: 1.04x faster                                                  |
| dask                     | 372 ms                                                 | 360 ms: 1.03x faster                                                   |
| async_tree_memoization   | 578 ms                                                 | 559 ms: 1.03x faster                                                   |
| pickle_list              | 5.08 us                                                | 4.92 us: 1.03x faster                                                  |
| unpickle_list            | 5.29 us                                                | 5.13 us: 1.03x faster                                                  |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 704 ms: 1.03x faster                                                   |
| logging_silent           | 104 ns                                                 | 101 ns: 1.03x faster                                                   |
| sqlglot_optimize         | 54.8 ms                                                | 53.4 ms: 1.03x faster                                                  |
| xml_etree_iterparse      | 107 ms                                                 | 104 ms: 1.03x faster                                                   |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.93 ms: 1.02x faster                                                  |
| xml_etree_parse          | 159 ms                                                 | 156 ms: 1.02x faster                                                   |
| gc_traversal             | 3.79 ms                                                | 3.72 ms: 1.02x faster                                                  |
| async_tree_none_tg       | 450 ms                                                 | 441 ms: 1.02x faster                                                   |
| bench_thread_pool        | 842 us                                                 | 828 us: 1.02x faster                                                   |
| json_loads               | 28.5 us                                                | 28.1 us: 1.01x faster                                                  |
| asyncio_tcp              | 491 ms                                                 | 484 ms: 1.01x faster                                                   |
| json                     | 5.26 ms                                                | 5.21 ms: 1.01x faster                                                  |
| spectral_norm            | 115 ms                                                 | 114 ms: 1.01x faster                                                   |
| go                       | 139 ms                                                 | 138 ms: 1.01x faster                                                   |
| pickle                   | 11.6 us                                                | 11.5 us: 1.00x faster                                                  |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.78 sec: 1.00x faster                                                 |
| nqueens                  | 83.3 ms                                                | 83.9 ms: 1.01x slower                                                  |
| json_dumps               | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                  |
| async_tree_io_tg         | 1.18 sec                                               | 1.20 sec: 1.01x slower                                                 |
| pycparser                | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| async_tree_io            | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                 |
| richards                 | 45.8 ms                                                | 47.4 ms: 1.03x slower                                                  |
| pidigits                 | 187 ms                                                 | 195 ms: 1.04x slower                                                   |
| regex_effbot             | 3.61 ms                                                | 3.77 ms: 1.04x slower                                                  |
| richards_super           | 51.5 ms                                                | 53.8 ms: 1.04x slower                                                  |
| regex_dna                | 212 ms                                                 | 224 ms: 1.06x slower                                                   |
| python_startup           | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| regex_v8                 | 23.1 ms                                                | 25.3 ms: 1.09x slower                                                  |
| telco                    | 7.10 ms                                                | 8.32 ms: 1.17x slower                                                  |
| python_startup_no_site   | 6.94 ms                                                | 8.70 ms: 1.25x slower                                                  |
| coverage                 | 72.7 ms                                                | 96.2 ms: 1.32x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.04x faster                                                           |

Benchmark hidden because not significant (8): async_tree_cpu_io_mixed_tg, sqlite_synth, scimark_sor, create_gc_cycles, async_tree_memoization_tg, bench_mp_pool, asyncio_websockets, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.93x