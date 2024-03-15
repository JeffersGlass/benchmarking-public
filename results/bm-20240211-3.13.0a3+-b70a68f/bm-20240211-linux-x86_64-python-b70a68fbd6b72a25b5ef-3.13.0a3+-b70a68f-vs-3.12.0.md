
# Results vs. 3.12.0

- fork: python
- ref: b70a68fbd6b72a25b5ef
- machine: linux-x86_64
- commit hash: b70a68f
- commit date: 2024-02-11
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 263 ms: 1.04x faster                                                   |
| chameleon      | 7.41 ms                                                | 6.89 ms: 1.08x faster                                                  |
| docutils       | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                 |
| tornado_http   | 103 ms                                                 | 94.6 ms: 1.08x faster                                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 430 ms: 1.10x faster                                                   |
| async_tree_memoization  | 578 ms                                                 | 557 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed | 726 ms                                                 | 703 ms: 1.03x faster                                                   |
| async_tree_none_tg      | 450 ms                                                 | 442 ms: 1.02x faster                                                   |
| async_tree_io_tg        | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                 |
| async_tree_io           | 1.16 sec                                               | 1.17 sec: 1.01x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 90.0 ms: 1.08x faster                                                  |
| float          | 84.7 ms                                                | 81.3 ms: 1.04x faster                                                  |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                                   |
| Geometric mean | (ref)                                                  | 1.04x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 129 ms: 1.15x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.67 ms: 1.02x slower                                                  |
| regex_dna      | 212 ms                                                 | 223 ms: 1.05x slower                                                   |
| regex_v8       | 23.1 ms                                                | 25.7 ms: 1.11x slower                                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.13 sec: 1.09x faster                                                 |
| pickle_pure_python   | 324 us                                                 | 301 us: 1.08x faster                                                   |
| unpickle_list        | 5.29 us                                                | 4.98 us: 1.06x faster                                                  |
| unpickle_pure_python | 230 us                                                 | 217 us: 1.06x faster                                                   |
| xml_etree_process    | 61.7 ms                                                | 58.3 ms: 1.06x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 85.6 ms: 1.04x faster                                                  |
| json_loads           | 28.5 us                                                | 27.7 us: 1.03x faster                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 106 ms: 1.01x faster                                                   |
| pickle_dict          | 35.5 us                                                | 35.3 us: 1.01x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 159 ms: 1.00x faster                                                   |
| json_dumps           | 10.4 ms                                                | 10.4 ms: 1.00x slower                                                  |
| pickle               | 11.6 us                                                | 11.8 us: 1.02x slower                                                  |
| pickle_list          | 5.08 us                                                | 5.25 us: 1.03x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.76 ms: 1.26x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.2 ms: 1.06x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 110 us: 1.43x faster                                                   |
| comprehensions           | 21.8 us                                                | 16.3 us: 1.33x faster                                                  |
| raytrace                 | 312 ms                                                 | 256 ms: 1.22x faster                                                   |
| deltablue                | 3.72 ms                                                | 3.16 ms: 1.17x faster                                                  |
| logging_format           | 7.23 us                                                | 6.19 us: 1.17x faster                                                  |
| crypto_pyaes             | 81.9 ms                                                | 70.7 ms: 1.16x faster                                                  |
| logging_simple           | 6.46 us                                                | 5.62 us: 1.15x faster                                                  |
| regex_compile            | 148 ms                                                 | 129 ms: 1.15x faster                                                   |
| sympy_sum                | 169 ms                                                 | 147 ms: 1.15x faster                                                   |
| scimark_monte_carlo      | 75.1 ms                                                | 65.7 ms: 1.14x faster                                                  |
| chaos                    | 67.0 ms                                                | 58.8 ms: 1.14x faster                                                  |
| sympy_str                | 300 ms                                                 | 268 ms: 1.12x faster                                                   |
| logging_silent           | 104 ns                                                 | 94.2 ns: 1.11x faster                                                  |
| unpack_sequence          | 54.0 ns                                                | 48.8 ns: 1.10x faster                                                  |
| deepcopy_reduce          | 3.35 us                                                | 3.04 us: 1.10x faster                                                  |
| async_tree_none          | 472 ms                                                 | 430 ms: 1.10x faster                                                   |
| sympy_integrate          | 21.4 ms                                                | 19.5 ms: 1.10x faster                                                  |
| tomli_loads              | 2.33 sec                                               | 2.13 sec: 1.09x faster                                                 |
| sqlglot_parse            | 1.36 ms                                                | 1.25 ms: 1.09x faster                                                  |
| tornado_http             | 103 ms                                                 | 94.6 ms: 1.08x faster                                                  |
| deepcopy                 | 371 us                                                 | 344 us: 1.08x faster                                                   |
| sqlglot_transpile        | 1.68 ms                                                | 1.56 ms: 1.08x faster                                                  |
| nbody                    | 97.0 ms                                                | 90.0 ms: 1.08x faster                                                  |
| pickle_pure_python       | 324 us                                                 | 301 us: 1.08x faster                                                   |
| pprint_safe_repr         | 776 ms                                                 | 721 ms: 1.08x faster                                                   |
| chameleon                | 7.41 ms                                                | 6.89 ms: 1.08x faster                                                  |
| deepcopy_memo            | 40.7 us                                                | 37.9 us: 1.08x faster                                                  |
| generators               | 31.2 ms                                                | 29.2 ms: 1.07x faster                                                  |
| pprint_pformat           | 1.57 sec                                               | 1.48 sec: 1.06x faster                                                 |
| unpickle_list            | 5.29 us                                                | 4.98 us: 1.06x faster                                                  |
| docutils                 | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                 |
| hexiom                   | 6.41 ms                                                | 6.05 ms: 1.06x faster                                                  |
| mako                     | 11.9 ms                                                | 11.2 ms: 1.06x faster                                                  |
| unpickle_pure_python     | 230 us                                                 | 217 us: 1.06x faster                                                   |
| xml_etree_process        | 61.7 ms                                                | 58.3 ms: 1.06x faster                                                  |
| pathlib                  | 19.3 ms                                                | 18.3 ms: 1.06x faster                                                  |
| fannkuch                 | 417 ms                                                 | 395 ms: 1.05x faster                                                   |
| dulwich_log              | 68.5 ms                                                | 65.0 ms: 1.05x faster                                                  |
| coroutines               | 23.2 ms                                                | 22.0 ms: 1.05x faster                                                  |
| sympy_expand             | 478 ms                                                 | 454 ms: 1.05x faster                                                   |
| scimark_fft              | 382 ms                                                 | 363 ms: 1.05x faster                                                   |
| scimark_lu               | 118 ms                                                 | 113 ms: 1.05x faster                                                   |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.83 ms: 1.05x faster                                                  |
| 2to3                     | 274 ms                                                 | 263 ms: 1.04x faster                                                   |
| float                    | 84.7 ms                                                | 81.3 ms: 1.04x faster                                                  |
| xml_etree_generate       | 89.2 ms                                                | 85.6 ms: 1.04x faster                                                  |
| meteor_contest           | 112 ms                                                 | 108 ms: 1.04x faster                                                   |
| async_tree_memoization   | 578 ms                                                 | 557 ms: 1.04x faster                                                   |
| json                     | 5.26 ms                                                | 5.07 ms: 1.04x faster                                                  |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 703 ms: 1.03x faster                                                   |
| sqlglot_normalize        | 110 ms                                                 | 107 ms: 1.03x faster                                                   |
| async_generators         | 463 ms                                                 | 449 ms: 1.03x faster                                                   |
| json_loads               | 28.5 us                                                | 27.7 us: 1.03x faster                                                  |
| bench_thread_pool        | 842 us                                                 | 818 us: 1.03x faster                                                   |
| dask                     | 372 ms                                                 | 362 ms: 1.03x faster                                                   |
| pyflate                  | 482 ms                                                 | 470 ms: 1.03x faster                                                   |
| spectral_norm            | 115 ms                                                 | 112 ms: 1.03x faster                                                   |
| nqueens                  | 83.3 ms                                                | 81.4 ms: 1.02x faster                                                  |
| mdp                      | 2.63 sec                                               | 2.58 sec: 1.02x faster                                                 |
| sqlglot_optimize         | 54.8 ms                                                | 53.8 ms: 1.02x faster                                                  |
| async_tree_none_tg       | 450 ms                                                 | 442 ms: 1.02x faster                                                   |
| sqlite_synth             | 2.83 us                                                | 2.79 us: 1.02x faster                                                  |
| pycparser                | 1.18 sec                                               | 1.16 sec: 1.01x faster                                                 |
| gc_traversal             | 3.79 ms                                                | 3.76 ms: 1.01x faster                                                  |
| xml_etree_iterparse      | 107 ms                                                 | 106 ms: 1.01x faster                                                   |
| asyncio_tcp              | 491 ms                                                 | 487 ms: 1.01x faster                                                   |
| pickle_dict              | 35.5 us                                                | 35.3 us: 1.01x faster                                                  |
| xml_etree_parse          | 159 ms                                                 | 159 ms: 1.00x faster                                                   |
| go                       | 139 ms                                                 | 139 ms: 1.00x faster                                                   |
| pidigits                 | 187 ms                                                 | 187 ms: 1.00x faster                                                   |
| json_dumps               | 10.4 ms                                                | 10.4 ms: 1.00x slower                                                  |
| async_tree_io_tg         | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                 |
| create_gc_cycles         | 1.48 ms                                                | 1.49 ms: 1.01x slower                                                  |
| async_tree_io            | 1.16 sec                                               | 1.17 sec: 1.01x slower                                                 |
| pickle                   | 11.6 us                                                | 11.8 us: 1.02x slower                                                  |
| regex_effbot             | 3.61 ms                                                | 3.67 ms: 1.02x slower                                                  |
| richards                 | 45.8 ms                                                | 46.9 ms: 1.02x slower                                                  |
| pickle_list              | 5.08 us                                                | 5.25 us: 1.03x slower                                                  |
| richards_super           | 51.5 ms                                                | 53.3 ms: 1.03x slower                                                  |
| regex_dna                | 212 ms                                                 | 223 ms: 1.05x slower                                                   |
| python_startup           | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| regex_v8                 | 23.1 ms                                                | 25.7 ms: 1.11x slower                                                  |
| telco                    | 7.10 ms                                                | 8.35 ms: 1.18x slower                                                  |
| python_startup_no_site   | 6.94 ms                                                | 8.76 ms: 1.26x slower                                                  |
| coverage                 | 72.7 ms                                                | 95.3 ms: 1.31x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.04x faster                                                           |

Benchmark hidden because not significant (8): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, scimark_sor, asyncio_websockets, asyncio_tcp_ssl, bench_mp_pool, unpickle, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.93x