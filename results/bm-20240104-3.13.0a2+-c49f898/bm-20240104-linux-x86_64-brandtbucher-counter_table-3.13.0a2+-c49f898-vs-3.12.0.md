
# Results vs. 3.12.0

- fork: brandtbucher
- ref: counter_table
- machine: linux-x86_64
- commit hash: c49f898
- commit date: 2024-01-04
- overall geometric mean: 1.04x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 266 ms: 1.03x faster                                                  |
| chameleon      | 7.41 ms                                                | 6.96 ms: 1.06x faster                                                 |
| docutils       | 2.77 sec                                               | 2.62 sec: 1.06x faster                                                |
| tornado_http   | 103 ms                                                 | 94.9 ms: 1.08x faster                                                 |
| Geometric mean | (ref)                                                  | 1.06x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 436 ms: 1.08x faster                                                  |
| async_tree_memoization  | 578 ms                                                 | 562 ms: 1.03x faster                                                  |
| async_tree_cpu_io_mixed | 726 ms                                                 | 707 ms: 1.03x faster                                                  |
| async_tree_none_tg      | 450 ms                                                 | 443 ms: 1.02x faster                                                  |
| async_tree_io_tg        | 1.18 sec                                               | 1.20 sec: 1.01x slower                                                |
| async_tree_io           | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                |
| Geometric mean          | (ref)                                                  | 1.01x faster                                                          |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 88.9 ms: 1.09x faster                                                 |
| float          | 84.7 ms                                                | 80.2 ms: 1.06x faster                                                 |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x slower                                                  |
| Geometric mean | (ref)                                                  | 1.05x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 131 ms: 1.13x faster                                                  |
| regex_dna      | 212 ms                                                 | 217 ms: 1.02x slower                                                  |
| regex_v8       | 23.1 ms                                                | 25.4 ms: 1.10x slower                                                 |
| Geometric mean | (ref)                                                  | 1.00x faster                                                          |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 295 us: 1.10x faster                                                  |
| tomli_loads          | 2.33 sec                                               | 2.13 sec: 1.09x faster                                                |
| unpickle_pure_python | 230 us                                                 | 218 us: 1.06x faster                                                  |
| pickle_list          | 5.08 us                                                | 4.87 us: 1.04x faster                                                 |
| xml_etree_process    | 61.7 ms                                                | 60.1 ms: 1.03x faster                                                 |
| pickle               | 11.6 us                                                | 11.3 us: 1.02x faster                                                 |
| xml_etree_generate   | 89.2 ms                                                | 87.2 ms: 1.02x faster                                                 |
| pickle_dict          | 35.5 us                                                | 34.9 us: 1.02x faster                                                 |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.02x faster                                                  |
| json_loads           | 28.5 us                                                | 28.2 us: 1.01x faster                                                 |
| xml_etree_iterparse  | 107 ms                                                 | 106 ms: 1.01x faster                                                  |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                          |

Benchmark hidden because not significant (2): unpickle, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                 |
| python_startup_no_site | 6.94 ms                                                | 8.82 ms: 1.27x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 10.9 ms: 1.09x faster                                                 |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 112 us: 1.42x faster                                                  |
| comprehensions           | 21.8 us                                                | 16.6 us: 1.32x faster                                                 |
| raytrace                 | 312 ms                                                 | 261 ms: 1.19x faster                                                  |
| logging_format           | 7.23 us                                                | 6.24 us: 1.16x faster                                                 |
| deltablue                | 3.72 ms                                                | 3.24 ms: 1.15x faster                                                 |
| logging_simple           | 6.46 us                                                | 5.64 us: 1.14x faster                                                 |
| crypto_pyaes             | 81.9 ms                                                | 71.5 ms: 1.14x faster                                                 |
| chaos                    | 67.0 ms                                                | 58.8 ms: 1.14x faster                                                 |
| sympy_sum                | 169 ms                                                 | 149 ms: 1.14x faster                                                  |
| regex_compile            | 148 ms                                                 | 131 ms: 1.13x faster                                                  |
| scimark_monte_carlo      | 75.1 ms                                                | 66.9 ms: 1.12x faster                                                 |
| sympy_str                | 300 ms                                                 | 270 ms: 1.11x faster                                                  |
| pickle_pure_python       | 324 us                                                 | 295 us: 1.10x faster                                                  |
| tomli_loads              | 2.33 sec                                               | 2.13 sec: 1.09x faster                                                |
| nbody                    | 97.0 ms                                                | 88.9 ms: 1.09x faster                                                 |
| mako                     | 11.9 ms                                                | 10.9 ms: 1.09x faster                                                 |
| unpack_sequence          | 54.0 ns                                                | 49.7 ns: 1.09x faster                                                 |
| sqlglot_parse            | 1.36 ms                                                | 1.25 ms: 1.09x faster                                                 |
| deepcopy_reduce          | 3.35 us                                                | 3.09 us: 1.08x faster                                                 |
| sympy_integrate          | 21.4 ms                                                | 19.8 ms: 1.08x faster                                                 |
| tornado_http             | 103 ms                                                 | 94.9 ms: 1.08x faster                                                 |
| async_tree_none          | 472 ms                                                 | 436 ms: 1.08x faster                                                  |
| coroutines               | 23.2 ms                                                | 21.5 ms: 1.08x faster                                                 |
| scimark_sor              | 129 ms                                                 | 121 ms: 1.07x faster                                                  |
| scimark_fft              | 382 ms                                                 | 357 ms: 1.07x faster                                                  |
| sqlglot_transpile        | 1.68 ms                                                | 1.58 ms: 1.07x faster                                                 |
| fannkuch                 | 417 ms                                                 | 392 ms: 1.06x faster                                                  |
| chameleon                | 7.41 ms                                                | 6.96 ms: 1.06x faster                                                 |
| deepcopy                 | 371 us                                                 | 350 us: 1.06x faster                                                  |
| docutils                 | 2.77 sec                                               | 2.62 sec: 1.06x faster                                                |
| float                    | 84.7 ms                                                | 80.2 ms: 1.06x faster                                                 |
| unpickle_pure_python     | 230 us                                                 | 218 us: 1.06x faster                                                  |
| deepcopy_memo            | 40.7 us                                                | 38.6 us: 1.06x faster                                                 |
| gc_traversal             | 3.79 ms                                                | 3.60 ms: 1.05x faster                                                 |
| pathlib                  | 19.3 ms                                                | 18.4 ms: 1.05x faster                                                 |
| generators               | 31.2 ms                                                | 29.7 ms: 1.05x faster                                                 |
| pprint_safe_repr         | 776 ms                                                 | 739 ms: 1.05x faster                                                  |
| spectral_norm            | 115 ms                                                 | 110 ms: 1.05x faster                                                  |
| sympy_expand             | 478 ms                                                 | 456 ms: 1.05x faster                                                  |
| pickle_list              | 5.08 us                                                | 4.87 us: 1.04x faster                                                 |
| pprint_pformat           | 1.57 sec                                               | 1.50 sec: 1.04x faster                                                |
| pyflate                  | 482 ms                                                 | 464 ms: 1.04x faster                                                  |
| sqlglot_normalize        | 110 ms                                                 | 107 ms: 1.04x faster                                                  |
| dulwich_log              | 68.5 ms                                                | 66.2 ms: 1.03x faster                                                 |
| 2to3                     | 274 ms                                                 | 266 ms: 1.03x faster                                                  |
| async_generators         | 463 ms                                                 | 450 ms: 1.03x faster                                                  |
| dask                     | 372 ms                                                 | 362 ms: 1.03x faster                                                  |
| xml_etree_process        | 61.7 ms                                                | 60.1 ms: 1.03x faster                                                 |
| async_tree_memoization   | 578 ms                                                 | 562 ms: 1.03x faster                                                  |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 707 ms: 1.03x faster                                                  |
| pickle                   | 11.6 us                                                | 11.3 us: 1.02x faster                                                 |
| hexiom                   | 6.41 ms                                                | 6.27 ms: 1.02x faster                                                 |
| xml_etree_generate       | 89.2 ms                                                | 87.2 ms: 1.02x faster                                                 |
| meteor_contest           | 112 ms                                                 | 110 ms: 1.02x faster                                                  |
| scimark_lu               | 118 ms                                                 | 116 ms: 1.02x faster                                                  |
| pickle_dict              | 35.5 us                                                | 34.9 us: 1.02x faster                                                 |
| async_tree_none_tg       | 450 ms                                                 | 443 ms: 1.02x faster                                                  |
| xml_etree_parse          | 159 ms                                                 | 157 ms: 1.02x faster                                                  |
| sqlglot_optimize         | 54.8 ms                                                | 54.1 ms: 1.01x faster                                                 |
| go                       | 139 ms                                                 | 138 ms: 1.01x faster                                                  |
| json_loads               | 28.5 us                                                | 28.2 us: 1.01x faster                                                 |
| create_gc_cycles         | 1.48 ms                                                | 1.47 ms: 1.01x faster                                                 |
| xml_etree_iterparse      | 107 ms                                                 | 106 ms: 1.01x faster                                                  |
| asyncio_tcp              | 491 ms                                                 | 488 ms: 1.01x faster                                                  |
| bench_thread_pool        | 842 us                                                 | 838 us: 1.00x faster                                                  |
| nqueens                  | 83.3 ms                                                | 83.1 ms: 1.00x faster                                                 |
| pidigits                 | 187 ms                                                 | 187 ms: 1.00x slower                                                  |
| sqlite_synth             | 2.83 us                                                | 2.85 us: 1.01x slower                                                 |
| pycparser                | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                |
| async_tree_io_tg         | 1.18 sec                                               | 1.20 sec: 1.01x slower                                                |
| json_dumps               | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                 |
| async_tree_io            | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                |
| regex_dna                | 212 ms                                                 | 217 ms: 1.02x slower                                                  |
| mdp                      | 2.63 sec                                               | 2.73 sec: 1.04x slower                                                |
| python_startup           | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                 |
| richards_super           | 51.5 ms                                                | 55.1 ms: 1.07x slower                                                 |
| richards                 | 45.8 ms                                                | 49.1 ms: 1.07x slower                                                 |
| regex_v8                 | 23.1 ms                                                | 25.4 ms: 1.10x slower                                                 |
| telco                    | 7.10 ms                                                | 8.21 ms: 1.16x slower                                                 |
| python_startup_no_site   | 6.94 ms                                                | 8.82 ms: 1.27x slower                                                 |
| coverage                 | 72.7 ms                                                | 95.4 ms: 1.31x slower                                                 |
| Geometric mean           | (ref)                                                  | 1.04x faster                                                          |

Benchmark hidden because not significant (12): json, async_tree_cpu_io_mixed_tg, unpickle, logging_silent, regex_effbot, bench_mp_pool, asyncio_tcp_ssl, unpickle_list, asyncio_websockets, scimark_sparse_mat_mult, async_tree_memoization_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.93x