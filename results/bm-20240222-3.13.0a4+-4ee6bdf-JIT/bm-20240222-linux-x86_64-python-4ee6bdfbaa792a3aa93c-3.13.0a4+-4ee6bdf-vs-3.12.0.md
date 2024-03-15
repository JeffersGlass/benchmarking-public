
# Results vs. 3.12.0

- fork: python
- ref: 4ee6bdfbaa792a3aa93c
- machine: linux-x86_64
- commit hash: 4ee6bdf
- commit date: 2024-02-22
- overall geometric mean: 1.03x slower \*
- HPT reliability: 99.23%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 288 ms: 1.05x slower                                                   |
| chameleon      | 7.41 ms                                                | 6.74 ms: 1.10x faster                                                  |
| docutils       | 2.77 sec                                               | 2.75 sec: 1.01x faster                                                 |
| tornado_http   | 103 ms                                                 | 97.3 ms: 1.05x faster                                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 437 ms: 1.08x faster                                                   |
| async_tree_cpu_io_mixed | 726 ms                                                 | 709 ms: 1.02x faster                                                   |
| async_tree_memoization  | 578 ms                                                 | 565 ms: 1.02x faster                                                   |
| async_tree_io_tg        | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| async_tree_io           | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (3): async_tree_none_tg, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 83.7 ms: 1.01x faster                                                  |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                                   |
| nbody          | 97.0 ms                                                | 100 ms: 1.04x slower                                                   |
| Geometric mean | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.63 ms: 1.01x slower                                                  |
| regex_v8       | 23.1 ms                                                | 24.4 ms: 1.06x slower                                                  |
| regex_dna      | 212 ms                                                 | 226 ms: 1.06x slower                                                   |
| regex_compile  | 148 ms                                                 | 169 ms: 1.14x slower                                                   |
| Geometric mean | (ref)                                                  | 1.06x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 295 us: 1.10x faster                                                   |
| unpickle             | 15.9 us                                                | 14.8 us: 1.07x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 59.2 ms: 1.04x faster                                                  |
| unpickle_list        | 5.29 us                                                | 5.08 us: 1.04x faster                                                  |
| json_loads           | 28.5 us                                                | 27.4 us: 1.04x faster                                                  |
| pickle_dict          | 35.5 us                                                | 34.2 us: 1.04x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 87.2 ms: 1.02x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.01x faster                                                   |
| tomli_loads          | 2.33 sec                                               | 2.30 sec: 1.01x faster                                                 |
| pickle               | 11.6 us                                                | 11.5 us: 1.01x faster                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 109 ms: 1.02x slower                                                   |
| pickle_list          | 5.08 us                                                | 5.20 us: 1.02x slower                                                  |
| unpickle_pure_python | 230 us                                                 | 254 us: 1.10x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 11.7 ms: 1.22x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 10.3 ms: 1.49x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.35x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 12.1 ms: 1.01x slower                                                  |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 111 us: 1.42x faster                                                   |
| logging_format           | 7.23 us                                                | 6.31 us: 1.15x faster                                                  |
| logging_simple           | 6.46 us                                                | 5.72 us: 1.13x faster                                                  |
| comprehensions           | 21.8 us                                                | 19.4 us: 1.12x faster                                                  |
| deepcopy_reduce          | 3.35 us                                                | 3.04 us: 1.10x faster                                                  |
| chameleon                | 7.41 ms                                                | 6.74 ms: 1.10x faster                                                  |
| pickle_pure_python       | 324 us                                                 | 295 us: 1.10x faster                                                   |
| async_tree_none          | 472 ms                                                 | 437 ms: 1.08x faster                                                   |
| logging_silent           | 104 ns                                                 | 97.3 ns: 1.07x faster                                                  |
| unpickle                 | 15.9 us                                                | 14.8 us: 1.07x faster                                                  |
| deepcopy                 | 371 us                                                 | 348 us: 1.07x faster                                                   |
| json                     | 5.26 ms                                                | 4.97 ms: 1.06x faster                                                  |
| tornado_http             | 103 ms                                                 | 97.3 ms: 1.05x faster                                                  |
| generators               | 31.2 ms                                                | 29.6 ms: 1.05x faster                                                  |
| crypto_pyaes             | 81.9 ms                                                | 77.7 ms: 1.05x faster                                                  |
| deltablue                | 3.72 ms                                                | 3.53 ms: 1.05x faster                                                  |
| scimark_fft              | 382 ms                                                 | 363 ms: 1.05x faster                                                   |
| coroutines               | 23.2 ms                                                | 22.1 ms: 1.05x faster                                                  |
| xml_etree_process        | 61.7 ms                                                | 59.2 ms: 1.04x faster                                                  |
| unpickle_list            | 5.29 us                                                | 5.08 us: 1.04x faster                                                  |
| sympy_sum                | 169 ms                                                 | 162 ms: 1.04x faster                                                   |
| json_loads               | 28.5 us                                                | 27.4 us: 1.04x faster                                                  |
| pathlib                  | 19.3 ms                                                | 18.6 ms: 1.04x faster                                                  |
| pickle_dict              | 35.5 us                                                | 34.2 us: 1.04x faster                                                  |
| sympy_str                | 300 ms                                                 | 291 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 709 ms: 1.02x faster                                                   |
| async_tree_memoization   | 578 ms                                                 | 565 ms: 1.02x faster                                                   |
| xml_etree_generate       | 89.2 ms                                                | 87.2 ms: 1.02x faster                                                  |
| deepcopy_memo            | 40.7 us                                                | 39.9 us: 1.02x faster                                                  |
| xml_etree_parse          | 159 ms                                                 | 157 ms: 1.01x faster                                                   |
| tomli_loads              | 2.33 sec                                               | 2.30 sec: 1.01x faster                                                 |
| float                    | 84.7 ms                                                | 83.7 ms: 1.01x faster                                                  |
| sympy_integrate          | 21.4 ms                                                | 21.2 ms: 1.01x faster                                                  |
| pickle                   | 11.6 us                                                | 11.5 us: 1.01x faster                                                  |
| sqlglot_normalize        | 110 ms                                                 | 109 ms: 1.01x faster                                                   |
| docutils                 | 2.77 sec                                               | 2.75 sec: 1.01x faster                                                 |
| sqlite_synth             | 2.83 us                                                | 2.82 us: 1.01x faster                                                  |
| asyncio_tcp              | 491 ms                                                 | 489 ms: 1.00x faster                                                   |
| pidigits                 | 187 ms                                                 | 187 ms: 1.00x faster                                                   |
| gc_traversal             | 3.79 ms                                                | 3.80 ms: 1.00x slower                                                  |
| meteor_contest           | 112 ms                                                 | 113 ms: 1.00x slower                                                   |
| regex_effbot             | 3.61 ms                                                | 3.63 ms: 1.01x slower                                                  |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                 |
| bench_thread_pool        | 842 us                                                 | 851 us: 1.01x slower                                                   |
| raytrace                 | 312 ms                                                 | 316 ms: 1.01x slower                                                   |
| mako                     | 11.9 ms                                                | 12.1 ms: 1.01x slower                                                  |
| async_generators         | 463 ms                                                 | 470 ms: 1.02x slower                                                   |
| xml_etree_iterparse      | 107 ms                                                 | 109 ms: 1.02x slower                                                   |
| create_gc_cycles         | 1.48 ms                                                | 1.50 ms: 1.02x slower                                                  |
| async_tree_io_tg         | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| pickle_list              | 5.08 us                                                | 5.20 us: 1.02x slower                                                  |
| async_tree_io            | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                 |
| scimark_sor              | 129 ms                                                 | 133 ms: 1.03x slower                                                   |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 5.23 ms: 1.03x slower                                                  |
| nbody                    | 97.0 ms                                                | 100 ms: 1.04x slower                                                   |
| chaos                    | 67.0 ms                                                | 69.4 ms: 1.04x slower                                                  |
| sympy_expand             | 478 ms                                                 | 497 ms: 1.04x slower                                                   |
| dulwich_log              | 68.5 ms                                                | 71.2 ms: 1.04x slower                                                  |
| 2to3                     | 274 ms                                                 | 288 ms: 1.05x slower                                                   |
| sqlglot_optimize         | 54.8 ms                                                | 57.9 ms: 1.06x slower                                                  |
| regex_v8                 | 23.1 ms                                                | 24.4 ms: 1.06x slower                                                  |
| fannkuch                 | 417 ms                                                 | 442 ms: 1.06x slower                                                   |
| regex_dna                | 212 ms                                                 | 226 ms: 1.06x slower                                                   |
| pycparser                | 1.18 sec                                               | 1.27 sec: 1.07x slower                                                 |
| mdp                      | 2.63 sec                                               | 2.83 sec: 1.08x slower                                                 |
| scimark_monte_carlo      | 75.1 ms                                                | 81.4 ms: 1.08x slower                                                  |
| spectral_norm            | 115 ms                                                 | 126 ms: 1.10x slower                                                   |
| unpickle_pure_python     | 230 us                                                 | 254 us: 1.10x slower                                                   |
| richards_super           | 51.5 ms                                                | 57.2 ms: 1.11x slower                                                  |
| richards                 | 45.8 ms                                                | 51.6 ms: 1.13x slower                                                  |
| pyflate                  | 482 ms                                                 | 543 ms: 1.13x slower                                                   |
| regex_compile            | 148 ms                                                 | 169 ms: 1.14x slower                                                   |
| scimark_lu               | 118 ms                                                 | 135 ms: 1.14x slower                                                   |
| pprint_safe_repr         | 776 ms                                                 | 889 ms: 1.15x slower                                                   |
| nqueens                  | 83.3 ms                                                | 95.5 ms: 1.15x slower                                                  |
| bench_mp_pool            | 24.0 ms                                                | 28.2 ms: 1.17x slower                                                  |
| telco                    | 7.10 ms                                                | 8.46 ms: 1.19x slower                                                  |
| python_startup           | 9.55 ms                                                | 11.7 ms: 1.22x slower                                                  |
| go                       | 139 ms                                                 | 171 ms: 1.22x slower                                                   |
| pprint_pformat           | 1.57 sec                                               | 1.92 sec: 1.22x slower                                                 |
| coverage                 | 72.7 ms                                                | 95.8 ms: 1.32x slower                                                  |
| hexiom                   | 6.41 ms                                                | 8.80 ms: 1.37x slower                                                  |
| python_startup_no_site   | 6.94 ms                                                | 10.3 ms: 1.49x slower                                                  |
| unpack_sequence          | 54.0 ns                                                | 159 ns: 2.96x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.03x slower                                                           |

Benchmark hidden because not significant (8): async_tree_none_tg, async_tree_cpu_io_mixed_tg, sqlglot_parse, sqlglot_transpile, asyncio_websockets, json_dumps, async_tree_memoization_tg, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.23% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.07x