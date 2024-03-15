
# Results vs. 3.12.0

- fork: python
- ref: e3dedeae7abbeda0cb3f
- machine: linux-x86_64
- commit hash: e3dedea
- commit date: 2024-02-24
- overall geometric mean: 1.05x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 263 ms: 1.04x faster                                                   |
| chameleon      | 7.41 ms                                                | 6.67 ms: 1.11x faster                                                  |
| docutils       | 2.77 sec                                               | 2.58 sec: 1.07x faster                                                 |
| tornado_http   | 103 ms                                                 | 94.5 ms: 1.09x faster                                                  |
| Geometric mean | (ref)                                                  | 1.08x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 433 ms: 1.09x faster                                                   |
| async_tree_memoization  | 578 ms                                                 | 556 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed | 726 ms                                                 | 703 ms: 1.03x faster                                                   |
| async_tree_none_tg      | 450 ms                                                 | 444 ms: 1.01x faster                                                   |
| async_tree_io_tg        | 1.18 sec                                               | 1.19 sec: 1.00x slower                                                 |
| async_tree_io           | 1.16 sec                                               | 1.17 sec: 1.01x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 88.7 ms: 1.09x faster                                                  |
| float          | 84.7 ms                                                | 80.1 ms: 1.06x faster                                                  |
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                                   |
| Geometric mean | (ref)                                                  | 1.05x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 130 ms: 1.14x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.49 ms: 1.03x faster                                                  |
| regex_dna      | 212 ms                                                 | 214 ms: 1.01x slower                                                   |
| regex_v8       | 23.1 ms                                                | 24.6 ms: 1.06x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 289 us: 1.12x faster                                                   |
| unpickle_pure_python | 230 us                                                 | 211 us: 1.09x faster                                                   |
| tomli_loads          | 2.33 sec                                               | 2.14 sec: 1.09x faster                                                 |
| xml_etree_process    | 61.7 ms                                                | 57.9 ms: 1.07x faster                                                  |
| unpickle             | 15.9 us                                                | 14.9 us: 1.07x faster                                                  |
| unpickle_list        | 5.29 us                                                | 4.98 us: 1.06x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 84.3 ms: 1.06x faster                                                  |
| json_loads           | 28.5 us                                                | 27.4 us: 1.04x faster                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 105 ms: 1.02x faster                                                   |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.02x faster                                                   |
| pickle_dict          | 35.5 us                                                | 35.8 us: 1.01x slower                                                  |
| pickle_list          | 5.08 us                                                | 5.21 us: 1.03x slower                                                  |
| pickle               | 11.6 us                                                | 12.1 us: 1.04x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                           |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.73 ms: 1.26x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 10.7 ms: 1.11x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-linux-x86_64-python-e3dedeae7abbeda0cb3f-3.13.0a4+-e3dedea |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 111 us: 1.42x faster                                                   |
| comprehensions           | 21.8 us                                                | 16.2 us: 1.35x faster                                                  |
| raytrace                 | 312 ms                                                 | 257 ms: 1.21x faster                                                   |
| deltablue                | 3.72 ms                                                | 3.13 ms: 1.19x faster                                                  |
| logging_format           | 7.23 us                                                | 6.16 us: 1.17x faster                                                  |
| crypto_pyaes             | 81.9 ms                                                | 70.5 ms: 1.16x faster                                                  |
| logging_simple           | 6.46 us                                                | 5.61 us: 1.15x faster                                                  |
| sympy_sum                | 169 ms                                                 | 147 ms: 1.15x faster                                                   |
| chaos                    | 67.0 ms                                                | 58.5 ms: 1.14x faster                                                  |
| scimark_monte_carlo      | 75.1 ms                                                | 66.0 ms: 1.14x faster                                                  |
| regex_compile            | 148 ms                                                 | 130 ms: 1.14x faster                                                   |
| deepcopy_memo            | 40.7 us                                                | 36.2 us: 1.13x faster                                                  |
| deepcopy_reduce          | 3.35 us                                                | 2.98 us: 1.12x faster                                                  |
| pickle_pure_python       | 324 us                                                 | 289 us: 1.12x faster                                                   |
| sympy_str                | 300 ms                                                 | 268 ms: 1.12x faster                                                   |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.54 ms: 1.11x faster                                                  |
| chameleon                | 7.41 ms                                                | 6.67 ms: 1.11x faster                                                  |
| mako                     | 11.9 ms                                                | 10.7 ms: 1.11x faster                                                  |
| deepcopy                 | 371 us                                                 | 337 us: 1.10x faster                                                   |
| sympy_integrate          | 21.4 ms                                                | 19.5 ms: 1.10x faster                                                  |
| sqlglot_parse            | 1.36 ms                                                | 1.24 ms: 1.10x faster                                                  |
| fannkuch                 | 417 ms                                                 | 381 ms: 1.10x faster                                                   |
| nbody                    | 97.0 ms                                                | 88.7 ms: 1.09x faster                                                  |
| unpickle_pure_python     | 230 us                                                 | 211 us: 1.09x faster                                                   |
| async_tree_none          | 472 ms                                                 | 433 ms: 1.09x faster                                                   |
| tomli_loads              | 2.33 sec                                               | 2.14 sec: 1.09x faster                                                 |
| tornado_http             | 103 ms                                                 | 94.5 ms: 1.09x faster                                                  |
| scimark_fft              | 382 ms                                                 | 352 ms: 1.08x faster                                                   |
| sqlglot_transpile        | 1.68 ms                                                | 1.56 ms: 1.08x faster                                                  |
| logging_silent           | 104 ns                                                 | 97.0 ns: 1.08x faster                                                  |
| pprint_safe_repr         | 776 ms                                                 | 720 ms: 1.08x faster                                                   |
| pprint_pformat           | 1.57 sec                                               | 1.46 sec: 1.08x faster                                                 |
| docutils                 | 2.77 sec                                               | 2.58 sec: 1.07x faster                                                 |
| pathlib                  | 19.3 ms                                                | 18.1 ms: 1.07x faster                                                  |
| hexiom                   | 6.41 ms                                                | 5.99 ms: 1.07x faster                                                  |
| generators               | 31.2 ms                                                | 29.2 ms: 1.07x faster                                                  |
| xml_etree_process        | 61.7 ms                                                | 57.9 ms: 1.07x faster                                                  |
| sympy_expand             | 478 ms                                                 | 449 ms: 1.07x faster                                                   |
| unpickle                 | 15.9 us                                                | 14.9 us: 1.07x faster                                                  |
| unpickle_list            | 5.29 us                                                | 4.98 us: 1.06x faster                                                  |
| float                    | 84.7 ms                                                | 80.1 ms: 1.06x faster                                                  |
| xml_etree_generate       | 89.2 ms                                                | 84.3 ms: 1.06x faster                                                  |
| spectral_norm            | 115 ms                                                 | 109 ms: 1.06x faster                                                   |
| scimark_sor              | 129 ms                                                 | 122 ms: 1.06x faster                                                   |
| json                     | 5.26 ms                                                | 4.98 ms: 1.06x faster                                                  |
| coroutines               | 23.2 ms                                                | 22.0 ms: 1.05x faster                                                  |
| pyflate                  | 482 ms                                                 | 458 ms: 1.05x faster                                                   |
| meteor_contest           | 112 ms                                                 | 107 ms: 1.05x faster                                                   |
| dulwich_log              | 68.5 ms                                                | 65.2 ms: 1.05x faster                                                  |
| scimark_lu               | 118 ms                                                 | 112 ms: 1.05x faster                                                   |
| sqlglot_normalize        | 110 ms                                                 | 105 ms: 1.05x faster                                                   |
| 2to3                     | 274 ms                                                 | 263 ms: 1.04x faster                                                   |
| mdp                      | 2.63 sec                                               | 2.52 sec: 1.04x faster                                                 |
| nqueens                  | 83.3 ms                                                | 80.0 ms: 1.04x faster                                                  |
| async_tree_memoization   | 578 ms                                                 | 556 ms: 1.04x faster                                                   |
| json_loads               | 28.5 us                                                | 27.4 us: 1.04x faster                                                  |
| bench_thread_pool        | 842 us                                                 | 813 us: 1.03x faster                                                   |
| regex_effbot             | 3.61 ms                                                | 3.49 ms: 1.03x faster                                                  |
| sqlglot_optimize         | 54.8 ms                                                | 53.0 ms: 1.03x faster                                                  |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 703 ms: 1.03x faster                                                   |
| async_generators         | 463 ms                                                 | 449 ms: 1.03x faster                                                   |
| go                       | 139 ms                                                 | 135 ms: 1.03x faster                                                   |
| pycparser                | 1.18 sec                                               | 1.15 sec: 1.03x faster                                                 |
| xml_etree_iterparse      | 107 ms                                                 | 105 ms: 1.02x faster                                                   |
| xml_etree_parse          | 159 ms                                                 | 157 ms: 1.02x faster                                                   |
| asyncio_tcp              | 491 ms                                                 | 484 ms: 1.01x faster                                                   |
| async_tree_none_tg       | 450 ms                                                 | 444 ms: 1.01x faster                                                   |
| sqlite_synth             | 2.83 us                                                | 2.81 us: 1.01x faster                                                  |
| pidigits                 | 187 ms                                                 | 188 ms: 1.00x slower                                                   |
| async_tree_io_tg         | 1.18 sec                                               | 1.19 sec: 1.00x slower                                                 |
| regex_dna                | 212 ms                                                 | 214 ms: 1.01x slower                                                   |
| pickle_dict              | 35.5 us                                                | 35.8 us: 1.01x slower                                                  |
| gc_traversal             | 3.79 ms                                                | 3.83 ms: 1.01x slower                                                  |
| create_gc_cycles         | 1.48 ms                                                | 1.49 ms: 1.01x slower                                                  |
| richards                 | 45.8 ms                                                | 46.3 ms: 1.01x slower                                                  |
| async_tree_io            | 1.16 sec                                               | 1.17 sec: 1.01x slower                                                 |
| richards_super           | 51.5 ms                                                | 52.5 ms: 1.02x slower                                                  |
| unpack_sequence          | 54.0 ns                                                | 55.0 ns: 1.02x slower                                                  |
| pickle_list              | 5.08 us                                                | 5.21 us: 1.03x slower                                                  |
| pickle                   | 11.6 us                                                | 12.1 us: 1.04x slower                                                  |
| python_startup           | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| regex_v8                 | 23.1 ms                                                | 24.6 ms: 1.06x slower                                                  |
| telco                    | 7.10 ms                                                | 8.34 ms: 1.17x slower                                                  |
| python_startup_no_site   | 6.94 ms                                                | 8.73 ms: 1.26x slower                                                  |
| coverage                 | 72.7 ms                                                | 94.4 ms: 1.30x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.05x faster                                                           |

Benchmark hidden because not significant (7): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, asyncio_websockets, bench_mp_pool, asyncio_tcp_ssl, json_dumps, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: 0.93x