
# Results vs. 3.12.0

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: linux-x86_64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.04x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 264 ms: 1.04x faster                                                   |
| chameleon      | 7.41 ms                                                | 6.90 ms: 1.07x faster                                                  |
| docutils       | 2.77 sec                                               | 2.59 sec: 1.07x faster                                                 |
| tornado_http   | 103 ms                                                 | 94.1 ms: 1.09x faster                                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 434 ms: 1.09x faster                                                   |
| async_tree_memoization  | 578 ms                                                 | 559 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed | 726 ms                                                 | 706 ms: 1.03x faster                                                   |
| async_tree_none_tg      | 450 ms                                                 | 438 ms: 1.03x faster                                                   |
| async_tree_io_tg        | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                 |
| async_tree_io           | 1.16 sec                                               | 1.17 sec: 1.02x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 87.4 ms: 1.11x faster                                                  |
| float          | 84.7 ms                                                | 79.7 ms: 1.06x faster                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                           |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 130 ms: 1.14x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.65 ms: 1.01x slower                                                  |
| regex_dna      | 212 ms                                                 | 223 ms: 1.05x slower                                                   |
| regex_v8       | 23.1 ms                                                | 25.0 ms: 1.08x slower                                                  |
| Geometric mean | (ref)                                                  | 1.00x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.13 sec: 1.10x faster                                                 |
| pickle_pure_python   | 324 us                                                 | 302 us: 1.07x faster                                                   |
| unpickle_pure_python | 230 us                                                 | 216 us: 1.07x faster                                                   |
| unpickle             | 15.9 us                                                | 14.9 us: 1.06x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 58.6 ms: 1.05x faster                                                  |
| unpickle_list        | 5.29 us                                                | 5.05 us: 1.05x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 85.1 ms: 1.05x faster                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 105 ms: 1.02x faster                                                   |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.02x faster                                                   |
| json_loads           | 28.5 us                                                | 28.1 us: 1.01x faster                                                  |
| pickle               | 11.6 us                                                | 11.7 us: 1.01x slower                                                  |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.02x slower                                                  |
| pickle_list          | 5.08 us                                                | 5.20 us: 1.02x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.71 ms: 1.26x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.2 ms: 1.06x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 111 us: 1.43x faster                                                   |
| comprehensions           | 21.8 us                                                | 16.0 us: 1.36x faster                                                  |
| unpack_sequence          | 54.0 ns                                                | 44.4 ns: 1.21x faster                                                  |
| raytrace                 | 312 ms                                                 | 262 ms: 1.19x faster                                                   |
| logging_format           | 7.23 us                                                | 6.18 us: 1.17x faster                                                  |
| crypto_pyaes             | 81.9 ms                                                | 70.0 ms: 1.17x faster                                                  |
| logging_simple           | 6.46 us                                                | 5.62 us: 1.15x faster                                                  |
| regex_compile            | 148 ms                                                 | 130 ms: 1.14x faster                                                   |
| sympy_sum                | 169 ms                                                 | 148 ms: 1.14x faster                                                   |
| deltablue                | 3.72 ms                                                | 3.26 ms: 1.14x faster                                                  |
| chaos                    | 67.0 ms                                                | 58.9 ms: 1.14x faster                                                  |
| scimark_monte_carlo      | 75.1 ms                                                | 67.6 ms: 1.11x faster                                                  |
| nbody                    | 97.0 ms                                                | 87.4 ms: 1.11x faster                                                  |
| deepcopy_reduce          | 3.35 us                                                | 3.02 us: 1.11x faster                                                  |
| sympy_integrate          | 21.4 ms                                                | 19.5 ms: 1.10x faster                                                  |
| tomli_loads              | 2.33 sec                                               | 2.13 sec: 1.10x faster                                                 |
| tornado_http             | 103 ms                                                 | 94.1 ms: 1.09x faster                                                  |
| sqlglot_parse            | 1.36 ms                                                | 1.25 ms: 1.09x faster                                                  |
| async_tree_none          | 472 ms                                                 | 434 ms: 1.09x faster                                                   |
| sympy_str                | 300 ms                                                 | 276 ms: 1.09x faster                                                   |
| deepcopy                 | 371 us                                                 | 344 us: 1.08x faster                                                   |
| chameleon                | 7.41 ms                                                | 6.90 ms: 1.07x faster                                                  |
| sqlglot_transpile        | 1.68 ms                                                | 1.57 ms: 1.07x faster                                                  |
| pickle_pure_python       | 324 us                                                 | 302 us: 1.07x faster                                                   |
| pprint_safe_repr         | 776 ms                                                 | 724 ms: 1.07x faster                                                   |
| docutils                 | 2.77 sec                                               | 2.59 sec: 1.07x faster                                                 |
| unpickle_pure_python     | 230 us                                                 | 216 us: 1.07x faster                                                   |
| unpickle                 | 15.9 us                                                | 14.9 us: 1.06x faster                                                  |
| float                    | 84.7 ms                                                | 79.7 ms: 1.06x faster                                                  |
| mako                     | 11.9 ms                                                | 11.2 ms: 1.06x faster                                                  |
| deepcopy_memo            | 40.7 us                                                | 38.4 us: 1.06x faster                                                  |
| generators               | 31.2 ms                                                | 29.4 ms: 1.06x faster                                                  |
| pyflate                  | 482 ms                                                 | 455 ms: 1.06x faster                                                   |
| pprint_pformat           | 1.57 sec                                               | 1.48 sec: 1.06x faster                                                 |
| pathlib                  | 19.3 ms                                                | 18.3 ms: 1.06x faster                                                  |
| hexiom                   | 6.41 ms                                                | 6.07 ms: 1.06x faster                                                  |
| scimark_fft              | 382 ms                                                 | 362 ms: 1.06x faster                                                   |
| async_generators         | 463 ms                                                 | 439 ms: 1.05x faster                                                   |
| xml_etree_process        | 61.7 ms                                                | 58.6 ms: 1.05x faster                                                  |
| spectral_norm            | 115 ms                                                 | 109 ms: 1.05x faster                                                   |
| scimark_lu               | 118 ms                                                 | 112 ms: 1.05x faster                                                   |
| dulwich_log              | 68.5 ms                                                | 65.3 ms: 1.05x faster                                                  |
| unpickle_list            | 5.29 us                                                | 5.05 us: 1.05x faster                                                  |
| xml_etree_generate       | 89.2 ms                                                | 85.1 ms: 1.05x faster                                                  |
| fannkuch                 | 417 ms                                                 | 399 ms: 1.05x faster                                                   |
| mdp                      | 2.63 sec                                               | 2.53 sec: 1.04x faster                                                 |
| meteor_contest           | 112 ms                                                 | 108 ms: 1.04x faster                                                   |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.87 ms: 1.04x faster                                                  |
| 2to3                     | 274 ms                                                 | 264 ms: 1.04x faster                                                   |
| dask                     | 372 ms                                                 | 359 ms: 1.03x faster                                                   |
| coroutines               | 23.2 ms                                                | 22.4 ms: 1.03x faster                                                  |
| nqueens                  | 83.3 ms                                                | 80.6 ms: 1.03x faster                                                  |
| async_tree_memoization   | 578 ms                                                 | 559 ms: 1.03x faster                                                   |
| logging_silent           | 104 ns                                                 | 102 ns: 1.03x faster                                                   |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 706 ms: 1.03x faster                                                   |
| gc_traversal             | 3.79 ms                                                | 3.69 ms: 1.03x faster                                                  |
| sympy_expand             | 478 ms                                                 | 465 ms: 1.03x faster                                                   |
| async_tree_none_tg       | 450 ms                                                 | 438 ms: 1.03x faster                                                   |
| sqlglot_normalize        | 110 ms                                                 | 108 ms: 1.02x faster                                                   |
| asyncio_tcp              | 491 ms                                                 | 480 ms: 1.02x faster                                                   |
| xml_etree_iterparse      | 107 ms                                                 | 105 ms: 1.02x faster                                                   |
| bench_thread_pool        | 842 us                                                 | 827 us: 1.02x faster                                                   |
| xml_etree_parse          | 159 ms                                                 | 157 ms: 1.02x faster                                                   |
| sqlglot_optimize         | 54.8 ms                                                | 53.9 ms: 1.02x faster                                                  |
| json                     | 5.26 ms                                                | 5.18 ms: 1.02x faster                                                  |
| json_loads               | 28.5 us                                                | 28.1 us: 1.01x faster                                                  |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.77 sec: 1.01x faster                                                 |
| scimark_sor              | 129 ms                                                 | 128 ms: 1.01x faster                                                   |
| go                       | 139 ms                                                 | 139 ms: 1.01x faster                                                   |
| create_gc_cycles         | 1.48 ms                                                | 1.47 ms: 1.00x faster                                                  |
| async_tree_io_tg         | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                 |
| pickle                   | 11.6 us                                                | 11.7 us: 1.01x slower                                                  |
| regex_effbot             | 3.61 ms                                                | 3.65 ms: 1.01x slower                                                  |
| pycparser                | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                 |
| json_dumps               | 10.4 ms                                                | 10.5 ms: 1.02x slower                                                  |
| async_tree_io            | 1.16 sec                                               | 1.17 sec: 1.02x slower                                                 |
| pickle_list              | 5.08 us                                                | 5.20 us: 1.02x slower                                                  |
| regex_dna                | 212 ms                                                 | 223 ms: 1.05x slower                                                   |
| richards                 | 45.8 ms                                                | 48.3 ms: 1.05x slower                                                  |
| python_startup           | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| richards_super           | 51.5 ms                                                | 55.0 ms: 1.07x slower                                                  |
| regex_v8                 | 23.1 ms                                                | 25.0 ms: 1.08x slower                                                  |
| telco                    | 7.10 ms                                                | 8.35 ms: 1.18x slower                                                  |
| python_startup_no_site   | 6.94 ms                                                | 8.71 ms: 1.26x slower                                                  |
| coverage                 | 72.7 ms                                                | 95.0 ms: 1.31x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.04x faster                                                           |

Benchmark hidden because not significant (8): async_tree_cpu_io_mixed_tg, bench_mp_pool, async_tree_memoization_tg, pidigits, pickle_dict, asyncio_websockets, sqlite_synth, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.93x