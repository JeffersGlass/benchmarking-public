# Results vs. 3.12.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: f58f8ce
- commit date: 2024-02-29
- overall geometric mean: 1.05x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 264 ms: 1.04x faster                                   |
| chameleon      | 7.41 ms                                                | 6.91 ms: 1.07x faster                                  |
| docutils       | 2.77 sec                                               | 2.59 sec: 1.07x faster                                 |
| tornado_http   | 103 ms                                                 | 94.8 ms: 1.08x faster                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 432 ms: 1.09x faster                                   |
| async_tree_memoization  | 578 ms                                                 | 556 ms: 1.04x faster                                   |
| async_tree_cpu_io_mixed | 726 ms                                                 | 704 ms: 1.03x faster                                   |
| async_tree_none_tg      | 450 ms                                                 | 445 ms: 1.01x faster                                   |
| async_tree_io_tg        | 1.18 sec                                               | 1.19 sec: 1.01x slower                                 |
| async_tree_io           | 1.16 sec                                               | 1.17 sec: 1.01x slower                                 |
| Geometric mean          | (ref)                                                  | 1.02x faster                                           |

Benchmark hidden because not significant (2): async_tree_memoization_tg, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 88.0 ms: 1.10x faster                                  |
| float          | 84.7 ms                                                | 80.4 ms: 1.05x faster                                  |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                   |
| Geometric mean | (ref)                                                  | 1.05x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 132 ms: 1.12x faster                                   |
| regex_effbot   | 3.61 ms                                                | 3.56 ms: 1.01x faster                                  |
| regex_dna      | 212 ms                                                 | 216 ms: 1.02x slower                                   |
| regex_v8       | 23.1 ms                                                | 24.6 ms: 1.06x slower                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 295 us: 1.10x faster                                   |
| unpickle             | 15.9 us                                                | 14.5 us: 1.10x faster                                  |
| tomli_loads          | 2.33 sec                                               | 2.14 sec: 1.09x faster                                 |
| unpickle_pure_python | 230 us                                                 | 214 us: 1.08x faster                                   |
| pickle_dict          | 35.5 us                                                | 33.1 us: 1.07x faster                                  |
| unpickle_list        | 5.29 us                                                | 4.95 us: 1.07x faster                                  |
| xml_etree_process    | 61.7 ms                                                | 58.3 ms: 1.06x faster                                  |
| xml_etree_generate   | 89.2 ms                                                | 85.0 ms: 1.05x faster                                  |
| pickle_list          | 5.08 us                                                | 4.91 us: 1.04x faster                                  |
| json_loads           | 28.5 us                                                | 27.6 us: 1.03x faster                                  |
| pickle               | 11.6 us                                                | 11.4 us: 1.02x faster                                  |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.02x faster                                   |
| xml_etree_iterparse  | 107 ms                                                 | 106 ms: 1.01x faster                                   |
| json_dumps           | 10.4 ms                                                | 10.3 ms: 1.01x faster                                  |
| Geometric mean       | (ref)                                                  | 1.05x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                  |
| python_startup_no_site | 6.94 ms                                                | 8.75 ms: 1.26x slower                                  |
| Geometric mean         | (ref)                                                  | 1.16x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|-----------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.4 ms: 1.04x faster                                  |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 110 us: 1.43x faster                                   |
| comprehensions           | 21.8 us                                                | 16.0 us: 1.36x faster                                  |
| raytrace                 | 312 ms                                                 | 263 ms: 1.19x faster                                   |
| logging_format           | 7.23 us                                                | 6.14 us: 1.18x faster                                  |
| crypto_pyaes             | 81.9 ms                                                | 69.6 ms: 1.18x faster                                  |
| deltablue                | 3.72 ms                                                | 3.16 ms: 1.17x faster                                  |
| logging_simple           | 6.46 us                                                | 5.60 us: 1.15x faster                                  |
| sympy_sum                | 169 ms                                                 | 148 ms: 1.14x faster                                   |
| unpack_sequence          | 54.0 ns                                                | 47.4 ns: 1.14x faster                                  |
| regex_compile            | 148 ms                                                 | 132 ms: 1.12x faster                                   |
| scimark_monte_carlo      | 75.1 ms                                                | 66.9 ms: 1.12x faster                                  |
| sympy_str                | 300 ms                                                 | 268 ms: 1.12x faster                                   |
| chaos                    | 67.0 ms                                                | 59.8 ms: 1.12x faster                                  |
| nbody                    | 97.0 ms                                                | 88.0 ms: 1.10x faster                                  |
| pickle_pure_python       | 324 us                                                 | 295 us: 1.10x faster                                   |
| deepcopy_reduce          | 3.35 us                                                | 3.05 us: 1.10x faster                                  |
| unpickle                 | 15.9 us                                                | 14.5 us: 1.10x faster                                  |
| sympy_integrate          | 21.4 ms                                                | 19.6 ms: 1.10x faster                                  |
| deepcopy_memo            | 40.7 us                                                | 37.2 us: 1.09x faster                                  |
| async_tree_none          | 472 ms                                                 | 432 ms: 1.09x faster                                   |
| tomli_loads              | 2.33 sec                                               | 2.14 sec: 1.09x faster                                 |
| sqlglot_parse            | 1.36 ms                                                | 1.25 ms: 1.09x faster                                  |
| tornado_http             | 103 ms                                                 | 94.8 ms: 1.08x faster                                  |
| deepcopy                 | 371 us                                                 | 344 us: 1.08x faster                                   |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.69 ms: 1.08x faster                                  |
| unpickle_pure_python     | 230 us                                                 | 214 us: 1.08x faster                                   |
| fannkuch                 | 417 ms                                                 | 388 ms: 1.07x faster                                   |
| pickle_dict              | 35.5 us                                                | 33.1 us: 1.07x faster                                  |
| hexiom                   | 6.41 ms                                                | 5.97 ms: 1.07x faster                                  |
| chameleon                | 7.41 ms                                                | 6.91 ms: 1.07x faster                                  |
| pathlib                  | 19.3 ms                                                | 18.0 ms: 1.07x faster                                  |
| scimark_lu               | 118 ms                                                 | 110 ms: 1.07x faster                                   |
| sqlglot_transpile        | 1.68 ms                                                | 1.57 ms: 1.07x faster                                  |
| pprint_safe_repr         | 776 ms                                                 | 724 ms: 1.07x faster                                   |
| docutils                 | 2.77 sec                                               | 2.59 sec: 1.07x faster                                 |
| unpickle_list            | 5.29 us                                                | 4.95 us: 1.07x faster                                  |
| generators               | 31.2 ms                                                | 29.3 ms: 1.07x faster                                  |
| scimark_fft              | 382 ms                                                 | 360 ms: 1.06x faster                                   |
| xml_etree_process        | 61.7 ms                                                | 58.3 ms: 1.06x faster                                  |
| nqueens                  | 83.3 ms                                                | 78.9 ms: 1.06x faster                                  |
| pprint_pformat           | 1.57 sec                                               | 1.49 sec: 1.05x faster                                 |
| float                    | 84.7 ms                                                | 80.4 ms: 1.05x faster                                  |
| sympy_expand             | 478 ms                                                 | 454 ms: 1.05x faster                                   |
| meteor_contest           | 112 ms                                                 | 107 ms: 1.05x faster                                   |
| spectral_norm            | 115 ms                                                 | 110 ms: 1.05x faster                                   |
| xml_etree_generate       | 89.2 ms                                                | 85.0 ms: 1.05x faster                                  |
| coroutines               | 23.2 ms                                                | 22.1 ms: 1.05x faster                                  |
| sqlglot_normalize        | 110 ms                                                 | 105 ms: 1.05x faster                                   |
| dulwich_log              | 68.5 ms                                                | 65.6 ms: 1.04x faster                                  |
| mako                     | 11.9 ms                                                | 11.4 ms: 1.04x faster                                  |
| json                     | 5.26 ms                                                | 5.05 ms: 1.04x faster                                  |
| 2to3                     | 274 ms                                                 | 264 ms: 1.04x faster                                   |
| scimark_sor              | 129 ms                                                 | 124 ms: 1.04x faster                                   |
| async_tree_memoization   | 578 ms                                                 | 556 ms: 1.04x faster                                   |
| pickle_list              | 5.08 us                                                | 4.91 us: 1.04x faster                                  |
| pyflate                  | 482 ms                                                 | 466 ms: 1.04x faster                                   |
| json_loads               | 28.5 us                                                | 27.6 us: 1.03x faster                                  |
| async_generators         | 463 ms                                                 | 448 ms: 1.03x faster                                   |
| bench_thread_pool        | 842 us                                                 | 816 us: 1.03x faster                                   |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 704 ms: 1.03x faster                                   |
| sqlglot_optimize         | 54.8 ms                                                | 53.4 ms: 1.03x faster                                  |
| logging_silent           | 104 ns                                                 | 102 ns: 1.02x faster                                   |
| pickle                   | 11.6 us                                                | 11.4 us: 1.02x faster                                  |
| xml_etree_parse          | 159 ms                                                 | 157 ms: 1.02x faster                                   |
| asyncio_tcp              | 491 ms                                                 | 483 ms: 1.02x faster                                   |
| regex_effbot             | 3.61 ms                                                | 3.56 ms: 1.01x faster                                  |
| gc_traversal             | 3.79 ms                                                | 3.75 ms: 1.01x faster                                  |
| async_tree_none_tg       | 450 ms                                                 | 445 ms: 1.01x faster                                   |
| xml_etree_iterparse      | 107 ms                                                 | 106 ms: 1.01x faster                                   |
| go                       | 139 ms                                                 | 138 ms: 1.01x faster                                   |
| json_dumps               | 10.4 ms                                                | 10.3 ms: 1.01x faster                                  |
| pidigits                 | 187 ms                                                 | 187 ms: 1.00x faster                                   |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.79 sec: 1.00x slower                                 |
| async_tree_io_tg         | 1.18 sec                                               | 1.19 sec: 1.01x slower                                 |
| create_gc_cycles         | 1.48 ms                                                | 1.50 ms: 1.01x slower                                  |
| async_tree_io            | 1.16 sec                                               | 1.17 sec: 1.01x slower                                 |
| sqlite_synth             | 2.83 us                                                | 2.88 us: 1.02x slower                                  |
| asyncio_websockets       | 551 ms                                                 | 560 ms: 1.02x slower                                   |
| mdp                      | 2.63 sec                                               | 2.68 sec: 1.02x slower                                 |
| regex_dna                | 212 ms                                                 | 216 ms: 1.02x slower                                   |
| pycparser                | 1.18 sec                                               | 1.21 sec: 1.02x slower                                 |
| richards_super           | 51.5 ms                                                | 52.9 ms: 1.03x slower                                  |
| richards                 | 45.8 ms                                                | 47.4 ms: 1.03x slower                                  |
| python_startup           | 9.55 ms                                                | 10.1 ms: 1.06x slower                                  |
| regex_v8                 | 23.1 ms                                                | 24.6 ms: 1.06x slower                                  |
| telco                    | 7.10 ms                                                | 8.20 ms: 1.15x slower                                  |
| python_startup_no_site   | 6.94 ms                                                | 8.75 ms: 1.26x slower                                  |
| coverage                 | 72.7 ms                                                | 93.0 ms: 1.28x slower                                  |
| Geometric mean           | (ref)                                                  | 1.05x faster                                           |

Benchmark hidden because not significant (4): async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, bench_mp_pool, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.93x