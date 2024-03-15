# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_mprotect
- machine: linux-x86_64
- commit hash: 41455df
- commit date: 2024-02-29
- overall geometric mean: 1.01x faster \*
- HPT reliability: 99.54%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 275 ms: 1.00x slower                                                    |
| chameleon      | 7.41 ms                                                | 6.77 ms: 1.10x faster                                                   |
| docutils       | 2.77 sec                                               | 2.70 sec: 1.03x faster                                                  |
| tornado_http   | 103 ms                                                 | 96.3 ms: 1.07x faster                                                   |
| Geometric mean | (ref)                                                  | 1.05x faster                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 439 ms: 1.08x faster                                                    |
| async_tree_cpu_io_mixed | 726 ms                                                 | 708 ms: 1.03x faster                                                    |
| async_tree_memoization  | 578 ms                                                 | 564 ms: 1.03x faster                                                    |
| async_tree_none_tg      | 450 ms                                                 | 445 ms: 1.01x faster                                                    |
| async_tree_io_tg        | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                  |
| async_tree_io           | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.01x faster                                                            |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 78.5 ms: 1.08x faster                                                   |
| nbody          | 97.0 ms                                                | 93.1 ms: 1.04x faster                                                   |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                                    |
| Geometric mean | (ref)                                                  | 1.04x faster                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 141 ms: 1.05x faster                                                    |
| regex_effbot   | 3.61 ms                                                | 3.82 ms: 1.06x slower                                                   |
| regex_v8       | 23.1 ms                                                | 24.6 ms: 1.06x slower                                                   |
| regex_dna      | 212 ms                                                 | 234 ms: 1.10x slower                                                    |
| Geometric mean | (ref)                                                  | 1.04x slower                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.04 sec: 1.14x faster                                                  |
| unpickle_list        | 5.29 us                                                | 4.70 us: 1.12x faster                                                   |
| unpickle             | 15.9 us                                                | 14.5 us: 1.09x faster                                                   |
| pickle_pure_python   | 324 us                                                 | 305 us: 1.06x faster                                                    |
| xml_etree_process    | 61.7 ms                                                | 58.6 ms: 1.05x faster                                                   |
| xml_etree_generate   | 89.2 ms                                                | 85.7 ms: 1.04x faster                                                   |
| json_loads           | 28.5 us                                                | 27.6 us: 1.03x faster                                                   |
| pickle_dict          | 35.5 us                                                | 34.4 us: 1.03x faster                                                   |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.02x faster                                                    |
| xml_etree_iterparse  | 107 ms                                                 | 106 ms: 1.01x faster                                                    |
| json_dumps           | 10.4 ms                                                | 10.3 ms: 1.01x faster                                                   |
| pickle_list          | 5.08 us                                                | 5.14 us: 1.01x slower                                                   |
| unpickle_pure_python | 230 us                                                 | 238 us: 1.03x slower                                                    |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                            |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 11.2 ms: 1.17x slower                                                   |
| python_startup_no_site | 6.94 ms                                                | 9.85 ms: 1.42x slower                                                   |
| Geometric mean         | (ref)                                                  | 1.29x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|-----------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 10.8 ms: 1.10x faster                                                   |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|--------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 110 us: 1.44x faster                                                    |
| comprehensions           | 21.8 us                                                | 17.2 us: 1.27x faster                                                   |
| logging_format           | 7.23 us                                                | 6.16 us: 1.17x faster                                                   |
| tomli_loads              | 2.33 sec                                               | 2.04 sec: 1.14x faster                                                  |
| logging_simple           | 6.46 us                                                | 5.65 us: 1.14x faster                                                   |
| scimark_fft              | 382 ms                                                 | 337 ms: 1.13x faster                                                    |
| crypto_pyaes             | 81.9 ms                                                | 72.8 ms: 1.12x faster                                                   |
| unpickle_list            | 5.29 us                                                | 4.70 us: 1.12x faster                                                   |
| mako                     | 11.9 ms                                                | 10.8 ms: 1.10x faster                                                   |
| deltablue                | 3.72 ms                                                | 3.38 ms: 1.10x faster                                                   |
| deepcopy_reduce          | 3.35 us                                                | 3.05 us: 1.10x faster                                                   |
| chameleon                | 7.41 ms                                                | 6.77 ms: 1.10x faster                                                   |
| unpickle                 | 15.9 us                                                | 14.5 us: 1.09x faster                                                   |
| sympy_sum                | 169 ms                                                 | 156 ms: 1.08x faster                                                    |
| float                    | 84.7 ms                                                | 78.5 ms: 1.08x faster                                                   |
| raytrace                 | 312 ms                                                 | 289 ms: 1.08x faster                                                    |
| sympy_str                | 300 ms                                                 | 279 ms: 1.08x faster                                                    |
| async_tree_none          | 472 ms                                                 | 439 ms: 1.08x faster                                                    |
| chaos                    | 67.0 ms                                                | 62.3 ms: 1.07x faster                                                   |
| deepcopy                 | 371 us                                                 | 348 us: 1.07x faster                                                    |
| tornado_http             | 103 ms                                                 | 96.3 ms: 1.07x faster                                                   |
| fannkuch                 | 417 ms                                                 | 392 ms: 1.06x faster                                                    |
| generators               | 31.2 ms                                                | 29.3 ms: 1.06x faster                                                   |
| scimark_monte_carlo      | 75.1 ms                                                | 70.7 ms: 1.06x faster                                                   |
| pickle_pure_python       | 324 us                                                 | 305 us: 1.06x faster                                                    |
| deepcopy_memo            | 40.7 us                                                | 38.5 us: 1.06x faster                                                   |
| sqlglot_parse            | 1.36 ms                                                | 1.29 ms: 1.05x faster                                                   |
| xml_etree_process        | 61.7 ms                                                | 58.6 ms: 1.05x faster                                                   |
| regex_compile            | 148 ms                                                 | 141 ms: 1.05x faster                                                    |
| pathlib                  | 19.3 ms                                                | 18.5 ms: 1.05x faster                                                   |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.85 ms: 1.04x faster                                                   |
| spectral_norm            | 115 ms                                                 | 110 ms: 1.04x faster                                                    |
| nbody                    | 97.0 ms                                                | 93.1 ms: 1.04x faster                                                   |
| json                     | 5.26 ms                                                | 5.05 ms: 1.04x faster                                                   |
| xml_etree_generate       | 89.2 ms                                                | 85.7 ms: 1.04x faster                                                   |
| meteor_contest           | 112 ms                                                 | 108 ms: 1.04x faster                                                    |
| sqlglot_transpile        | 1.68 ms                                                | 1.63 ms: 1.04x faster                                                   |
| json_loads               | 28.5 us                                                | 27.6 us: 1.03x faster                                                   |
| asyncio_tcp              | 491 ms                                                 | 475 ms: 1.03x faster                                                    |
| pprint_safe_repr         | 776 ms                                                 | 751 ms: 1.03x faster                                                    |
| pickle_dict              | 35.5 us                                                | 34.4 us: 1.03x faster                                                   |
| sqlglot_normalize        | 110 ms                                                 | 107 ms: 1.03x faster                                                    |
| sympy_integrate          | 21.4 ms                                                | 20.8 ms: 1.03x faster                                                   |
| docutils                 | 2.77 sec                                               | 2.70 sec: 1.03x faster                                                  |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 708 ms: 1.03x faster                                                    |
| async_tree_memoization   | 578 ms                                                 | 564 ms: 1.03x faster                                                    |
| pyflate                  | 482 ms                                                 | 471 ms: 1.02x faster                                                    |
| logging_silent           | 104 ns                                                 | 102 ns: 1.02x faster                                                    |
| coroutines               | 23.2 ms                                                | 22.7 ms: 1.02x faster                                                   |
| xml_etree_parse          | 159 ms                                                 | 157 ms: 1.02x faster                                                    |
| pprint_pformat           | 1.57 sec                                               | 1.55 sec: 1.01x faster                                                  |
| scimark_sor              | 129 ms                                                 | 127 ms: 1.01x faster                                                    |
| sympy_expand             | 478 ms                                                 | 473 ms: 1.01x faster                                                    |
| async_tree_none_tg       | 450 ms                                                 | 445 ms: 1.01x faster                                                    |
| xml_etree_iterparse      | 107 ms                                                 | 106 ms: 1.01x faster                                                    |
| json_dumps               | 10.4 ms                                                | 10.3 ms: 1.01x faster                                                   |
| async_generators         | 463 ms                                                 | 460 ms: 1.01x faster                                                    |
| pidigits                 | 187 ms                                                 | 187 ms: 1.00x faster                                                    |
| 2to3                     | 274 ms                                                 | 275 ms: 1.00x slower                                                    |
| gc_traversal             | 3.79 ms                                                | 3.80 ms: 1.00x slower                                                   |
| dulwich_log              | 68.5 ms                                                | 68.7 ms: 1.00x slower                                                   |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                  |
| pickle_list              | 5.08 us                                                | 5.14 us: 1.01x slower                                                   |
| sqlglot_optimize         | 54.8 ms                                                | 55.5 ms: 1.01x slower                                                   |
| async_tree_io_tg         | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                  |
| async_tree_io            | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                  |
| pycparser                | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                  |
| create_gc_cycles         | 1.48 ms                                                | 1.51 ms: 1.03x slower                                                   |
| unpickle_pure_python     | 230 us                                                 | 238 us: 1.03x slower                                                    |
| mdp                      | 2.63 sec                                               | 2.76 sec: 1.05x slower                                                  |
| regex_effbot             | 3.61 ms                                                | 3.82 ms: 1.06x slower                                                   |
| regex_v8                 | 23.1 ms                                                | 24.6 ms: 1.06x slower                                                   |
| nqueens                  | 83.3 ms                                                | 89.8 ms: 1.08x slower                                                   |
| hexiom                   | 6.41 ms                                                | 7.01 ms: 1.09x slower                                                   |
| scimark_lu               | 118 ms                                                 | 129 ms: 1.09x slower                                                    |
| regex_dna                | 212 ms                                                 | 234 ms: 1.10x slower                                                    |
| go                       | 139 ms                                                 | 155 ms: 1.11x slower                                                    |
| python_startup           | 9.55 ms                                                | 11.2 ms: 1.17x slower                                                   |
| telco                    | 7.10 ms                                                | 8.36 ms: 1.18x slower                                                   |
| coverage                 | 72.7 ms                                                | 96.4 ms: 1.33x slower                                                   |
| python_startup_no_site   | 6.94 ms                                                | 9.85 ms: 1.42x slower                                                   |
| dask                     | 372 ms                                                 | 530 ms: 1.43x slower                                                    |
| unpack_sequence          | 54.0 ns                                                | 96.7 ns: 1.79x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.01x faster                                                            |

Benchmark hidden because not significant (10): richards, async_tree_cpu_io_mixed_tg, bench_thread_pool, bench_mp_pool, async_tree_memoization_tg, asyncio_websockets, richards_super, sqlite_synth, pickle, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.54% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.06x