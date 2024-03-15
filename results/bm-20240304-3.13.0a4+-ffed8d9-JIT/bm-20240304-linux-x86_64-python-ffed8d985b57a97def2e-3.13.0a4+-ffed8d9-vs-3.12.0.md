# Results vs. 3.12.0

- fork: python
- ref: ffed8d985b57a97def2e
- machine: linux-x86_64
- commit hash: ffed8d9
- commit date: 2024-03-04
- overall geometric mean: 1.01x faster \*
- HPT reliability: 99.43%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.16x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 276 ms: 1.01x slower                                                   |
| chameleon      | 7.41 ms                                                | 6.76 ms: 1.10x faster                                                  |
| docutils       | 2.77 sec                                               | 2.70 sec: 1.03x faster                                                 |
| tornado_http   | 103 ms                                                 | 97.0 ms: 1.06x faster                                                  |
| Geometric mean | (ref)                                                  | 1.04x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 437 ms: 1.08x faster                                                   |
| async_tree_memoization  | 578 ms                                                 | 561 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed | 726 ms                                                 | 709 ms: 1.02x faster                                                   |
| async_tree_none_tg      | 450 ms                                                 | 448 ms: 1.00x faster                                                   |
| async_tree_io_tg        | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| async_tree_io           | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 79.2 ms: 1.07x faster                                                  |
| nbody          | 97.0 ms                                                | 95.4 ms: 1.02x faster                                                  |
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                                   |
| Geometric mean | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 143 ms: 1.04x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.67 ms: 1.02x slower                                                  |
| regex_dna      | 212 ms                                                 | 226 ms: 1.06x slower                                                   |
| regex_v8       | 23.1 ms                                                | 25.2 ms: 1.09x slower                                                  |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.02 sec: 1.15x faster                                                 |
| unpickle_list        | 5.29 us                                                | 4.90 us: 1.08x faster                                                  |
| unpickle             | 15.9 us                                                | 14.9 us: 1.06x faster                                                  |
| pickle_pure_python   | 324 us                                                 | 305 us: 1.06x faster                                                   |
| xml_etree_process    | 61.7 ms                                                | 58.7 ms: 1.05x faster                                                  |
| json_loads           | 28.5 us                                                | 27.4 us: 1.04x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 86.2 ms: 1.03x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                                   |
| pickle_dict          | 35.5 us                                                | 34.9 us: 1.02x faster                                                  |
| unpickle_pure_python | 230 us                                                 | 233 us: 1.01x slower                                                   |
| pickle_list          | 5.08 us                                                | 5.16 us: 1.02x slower                                                  |
| pickle               | 11.6 us                                                | 11.8 us: 1.02x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (2): xml_etree_iterparse, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.3 ms: 1.29x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 10.9 ms: 1.57x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.42x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 10.8 ms: 1.10x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 110 us: 1.43x faster                                                   |
| comprehensions           | 21.8 us                                                | 17.0 us: 1.28x faster                                                  |
| logging_format           | 7.23 us                                                | 6.23 us: 1.16x faster                                                  |
| tomli_loads              | 2.33 sec                                               | 2.02 sec: 1.15x faster                                                 |
| logging_simple           | 6.46 us                                                | 5.67 us: 1.14x faster                                                  |
| scimark_fft              | 382 ms                                                 | 341 ms: 1.12x faster                                                   |
| crypto_pyaes             | 81.9 ms                                                | 73.9 ms: 1.11x faster                                                  |
| deltablue                | 3.72 ms                                                | 3.38 ms: 1.10x faster                                                  |
| mako                     | 11.9 ms                                                | 10.8 ms: 1.10x faster                                                  |
| chameleon                | 7.41 ms                                                | 6.76 ms: 1.10x faster                                                  |
| deepcopy_reduce          | 3.35 us                                                | 3.06 us: 1.09x faster                                                  |
| raytrace                 | 312 ms                                                 | 288 ms: 1.09x faster                                                   |
| unpickle_list            | 5.29 us                                                | 4.90 us: 1.08x faster                                                  |
| async_tree_none          | 472 ms                                                 | 437 ms: 1.08x faster                                                   |
| sympy_sum                | 169 ms                                                 | 157 ms: 1.08x faster                                                   |
| chaos                    | 67.0 ms                                                | 62.4 ms: 1.07x faster                                                  |
| sympy_str                | 300 ms                                                 | 280 ms: 1.07x faster                                                   |
| float                    | 84.7 ms                                                | 79.2 ms: 1.07x faster                                                  |
| fannkuch                 | 417 ms                                                 | 392 ms: 1.06x faster                                                   |
| scimark_monte_carlo      | 75.1 ms                                                | 70.6 ms: 1.06x faster                                                  |
| unpickle                 | 15.9 us                                                | 14.9 us: 1.06x faster                                                  |
| pickle_pure_python       | 324 us                                                 | 305 us: 1.06x faster                                                   |
| generators               | 31.2 ms                                                | 29.4 ms: 1.06x faster                                                  |
| deepcopy                 | 371 us                                                 | 350 us: 1.06x faster                                                   |
| tornado_http             | 103 ms                                                 | 97.0 ms: 1.06x faster                                                  |
| pathlib                  | 19.3 ms                                                | 18.3 ms: 1.05x faster                                                  |
| sqlglot_parse            | 1.36 ms                                                | 1.29 ms: 1.05x faster                                                  |
| xml_etree_process        | 61.7 ms                                                | 58.7 ms: 1.05x faster                                                  |
| deepcopy_memo            | 40.7 us                                                | 38.9 us: 1.05x faster                                                  |
| meteor_contest           | 112 ms                                                 | 107 ms: 1.05x faster                                                   |
| json                     | 5.26 ms                                                | 5.03 ms: 1.04x faster                                                  |
| pprint_safe_repr         | 776 ms                                                 | 745 ms: 1.04x faster                                                   |
| regex_compile            | 148 ms                                                 | 143 ms: 1.04x faster                                                   |
| sqlglot_normalize        | 110 ms                                                 | 106 ms: 1.04x faster                                                   |
| logging_silent           | 104 ns                                                 | 101 ns: 1.04x faster                                                   |
| json_loads               | 28.5 us                                                | 27.4 us: 1.04x faster                                                  |
| xml_etree_generate       | 89.2 ms                                                | 86.2 ms: 1.03x faster                                                  |
| sqlglot_transpile        | 1.68 ms                                                | 1.63 ms: 1.03x faster                                                  |
| async_tree_memoization   | 578 ms                                                 | 561 ms: 1.03x faster                                                   |
| pyflate                  | 482 ms                                                 | 469 ms: 1.03x faster                                                   |
| docutils                 | 2.77 sec                                               | 2.70 sec: 1.03x faster                                                 |
| sympy_integrate          | 21.4 ms                                                | 20.9 ms: 1.03x faster                                                  |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 709 ms: 1.02x faster                                                   |
| asyncio_tcp              | 491 ms                                                 | 479 ms: 1.02x faster                                                   |
| coroutines               | 23.2 ms                                                | 22.7 ms: 1.02x faster                                                  |
| spectral_norm            | 115 ms                                                 | 112 ms: 1.02x faster                                                   |
| xml_etree_parse          | 159 ms                                                 | 156 ms: 1.02x faster                                                   |
| pickle_dict              | 35.5 us                                                | 34.9 us: 1.02x faster                                                  |
| pprint_pformat           | 1.57 sec                                               | 1.54 sec: 1.02x faster                                                 |
| scimark_sor              | 129 ms                                                 | 127 ms: 1.02x faster                                                   |
| nbody                    | 97.0 ms                                                | 95.4 ms: 1.02x faster                                                  |
| sqlite_synth             | 2.83 us                                                | 2.79 us: 1.01x faster                                                  |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 5.01 ms: 1.01x faster                                                  |
| mdp                      | 2.63 sec                                               | 2.61 sec: 1.01x faster                                                 |
| sympy_expand             | 478 ms                                                 | 475 ms: 1.01x faster                                                   |
| dulwich_log              | 68.5 ms                                                | 68.1 ms: 1.01x faster                                                  |
| async_tree_none_tg       | 450 ms                                                 | 448 ms: 1.00x faster                                                   |
| pidigits                 | 187 ms                                                 | 188 ms: 1.00x slower                                                   |
| asyncio_websockets       | 551 ms                                                 | 554 ms: 1.00x slower                                                   |
| bench_thread_pool        | 842 us                                                 | 846 us: 1.01x slower                                                   |
| 2to3                     | 274 ms                                                 | 276 ms: 1.01x slower                                                   |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                 |
| richards_super           | 51.5 ms                                                | 52.2 ms: 1.01x slower                                                  |
| unpickle_pure_python     | 230 us                                                 | 233 us: 1.01x slower                                                   |
| sqlglot_optimize         | 54.8 ms                                                | 55.6 ms: 1.02x slower                                                  |
| async_tree_io_tg         | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| create_gc_cycles         | 1.48 ms                                                | 1.50 ms: 1.02x slower                                                  |
| pickle_list              | 5.08 us                                                | 5.16 us: 1.02x slower                                                  |
| pickle                   | 11.6 us                                                | 11.8 us: 1.02x slower                                                  |
| regex_effbot             | 3.61 ms                                                | 3.67 ms: 1.02x slower                                                  |
| async_tree_io            | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                 |
| pycparser                | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| gc_traversal             | 3.79 ms                                                | 4.03 ms: 1.06x slower                                                  |
| regex_dna                | 212 ms                                                 | 226 ms: 1.06x slower                                                   |
| nqueens                  | 83.3 ms                                                | 90.2 ms: 1.08x slower                                                  |
| hexiom                   | 6.41 ms                                                | 6.95 ms: 1.08x slower                                                  |
| regex_v8                 | 23.1 ms                                                | 25.2 ms: 1.09x slower                                                  |
| scimark_lu               | 118 ms                                                 | 130 ms: 1.10x slower                                                   |
| go                       | 139 ms                                                 | 156 ms: 1.11x slower                                                   |
| bench_mp_pool            | 24.0 ms                                                | 28.0 ms: 1.16x slower                                                  |
| telco                    | 7.10 ms                                                | 8.45 ms: 1.19x slower                                                  |
| python_startup           | 9.55 ms                                                | 12.3 ms: 1.29x slower                                                  |
| coverage                 | 72.7 ms                                                | 97.0 ms: 1.34x slower                                                  |
| dask                     | 372 ms                                                 | 532 ms: 1.43x slower                                                   |
| python_startup_no_site   | 6.94 ms                                                | 10.9 ms: 1.57x slower                                                  |
| unpack_sequence          | 54.0 ns                                                | 85.0 ns: 1.58x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (7): xml_etree_iterparse, async_tree_cpu_io_mixed_tg, json_dumps, async_generators, async_tree_memoization_tg, richards, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.43% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.16x