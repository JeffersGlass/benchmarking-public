
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_ghccc
- machine: linux-x86_64
- commit hash: 61c470b
- commit date: 2024-02-03
- overall geometric mean: 1.01x faster \*
- HPT reliability: 89.80%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| chameleon      | 7.41 ms                                                | 7.04 ms: 1.05x faster                                                |
| docutils       | 2.77 sec                                               | 2.65 sec: 1.05x faster                                               |
| tornado_http   | 103 ms                                                 | 97.6 ms: 1.05x faster                                                |
| Geometric mean | (ref)                                                  | 1.04x faster                                                         |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 439 ms: 1.08x faster                                                 |
| async_tree_memoization  | 578 ms                                                 | 565 ms: 1.02x faster                                                 |
| async_tree_cpu_io_mixed | 726 ms                                                 | 711 ms: 1.02x faster                                                 |
| async_tree_none_tg      | 450 ms                                                 | 448 ms: 1.00x faster                                                 |
| async_tree_io_tg        | 1.18 sec                                               | 1.19 sec: 1.01x slower                                               |
| async_tree_io           | 1.16 sec                                               | 1.18 sec: 1.02x slower                                               |
| Geometric mean          | (ref)                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 88.2 ms: 1.10x faster                                                |
| float          | 84.7 ms                                                | 81.7 ms: 1.04x faster                                                |
| Geometric mean | (ref)                                                  | 1.04x faster                                                         |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 140 ms: 1.06x faster                                                 |
| regex_effbot   | 3.61 ms                                                | 3.58 ms: 1.01x faster                                                |
| regex_dna      | 212 ms                                                 | 224 ms: 1.05x slower                                                 |
| regex_v8       | 23.1 ms                                                | 25.6 ms: 1.11x slower                                                |
| Geometric mean | (ref)                                                  | 1.02x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.14 sec: 1.09x faster                                               |
| pickle_pure_python   | 324 us                                                 | 300 us: 1.08x faster                                                 |
| unpickle_list        | 5.29 us                                                | 4.98 us: 1.06x faster                                                |
| xml_etree_process    | 61.7 ms                                                | 58.4 ms: 1.06x faster                                                |
| xml_etree_generate   | 89.2 ms                                                | 86.4 ms: 1.03x faster                                                |
| xml_etree_parse      | 159 ms                                                 | 155 ms: 1.03x faster                                                 |
| unpickle             | 15.9 us                                                | 15.5 us: 1.02x faster                                                |
| unpickle_pure_python | 230 us                                                 | 226 us: 1.02x faster                                                 |
| pickle_list          | 5.08 us                                                | 4.99 us: 1.02x faster                                                |
| pickle_dict          | 35.5 us                                                | 35.1 us: 1.01x faster                                                |
| xml_etree_iterparse  | 107 ms                                                 | 106 ms: 1.01x faster                                                 |
| pickle               | 11.6 us                                                | 11.5 us: 1.01x faster                                                |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                         |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                |
| python_startup_no_site | 6.94 ms                                                | 8.77 ms: 1.26x slower                                                |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.9 ms: 1.00x slower                                                |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 112 us: 1.41x faster                                                 |
| comprehensions           | 21.8 us                                                | 18.6 us: 1.17x faster                                                |
| unpack_sequence          | 54.0 ns                                                | 47.2 ns: 1.14x faster                                                |
| crypto_pyaes             | 81.9 ms                                                | 72.5 ms: 1.13x faster                                                |
| logging_format           | 7.23 us                                                | 6.49 us: 1.11x faster                                                |
| raytrace                 | 312 ms                                                 | 281 ms: 1.11x faster                                                 |
| nbody                    | 97.0 ms                                                | 88.2 ms: 1.10x faster                                                |
| logging_simple           | 6.46 us                                                | 5.88 us: 1.10x faster                                                |
| scimark_fft              | 382 ms                                                 | 349 ms: 1.09x faster                                                 |
| tomli_loads              | 2.33 sec                                               | 2.14 sec: 1.09x faster                                               |
| deepcopy_reduce          | 3.35 us                                                | 3.09 us: 1.08x faster                                                |
| pickle_pure_python       | 324 us                                                 | 300 us: 1.08x faster                                                 |
| async_tree_none          | 472 ms                                                 | 439 ms: 1.08x faster                                                 |
| pathlib                  | 19.3 ms                                                | 18.1 ms: 1.07x faster                                                |
| regex_compile            | 148 ms                                                 | 140 ms: 1.06x faster                                                 |
| deepcopy                 | 371 us                                                 | 349 us: 1.06x faster                                                 |
| unpickle_list            | 5.29 us                                                | 4.98 us: 1.06x faster                                                |
| sqlglot_parse            | 1.36 ms                                                | 1.28 ms: 1.06x faster                                                |
| xml_etree_process        | 61.7 ms                                                | 58.4 ms: 1.06x faster                                                |
| sympy_str                | 300 ms                                                 | 284 ms: 1.06x faster                                                 |
| gc_traversal             | 3.79 ms                                                | 3.59 ms: 1.06x faster                                                |
| sympy_sum                | 169 ms                                                 | 160 ms: 1.05x faster                                                 |
| chameleon                | 7.41 ms                                                | 7.04 ms: 1.05x faster                                                |
| tornado_http             | 103 ms                                                 | 97.6 ms: 1.05x faster                                                |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.81 ms: 1.05x faster                                                |
| generators               | 31.2 ms                                                | 29.7 ms: 1.05x faster                                                |
| scimark_lu               | 118 ms                                                 | 113 ms: 1.05x faster                                                 |
| docutils                 | 2.77 sec                                               | 2.65 sec: 1.05x faster                                               |
| sqlglot_transpile        | 1.68 ms                                                | 1.62 ms: 1.04x faster                                                |
| float                    | 84.7 ms                                                | 81.7 ms: 1.04x faster                                                |
| xml_etree_generate       | 89.2 ms                                                | 86.4 ms: 1.03x faster                                                |
| deepcopy_memo            | 40.7 us                                                | 39.5 us: 1.03x faster                                                |
| coroutines               | 23.2 ms                                                | 22.5 ms: 1.03x faster                                                |
| xml_etree_parse          | 159 ms                                                 | 155 ms: 1.03x faster                                                 |
| meteor_contest           | 112 ms                                                 | 109 ms: 1.03x faster                                                 |
| scimark_monte_carlo      | 75.1 ms                                                | 73.2 ms: 1.03x faster                                                |
| logging_silent           | 104 ns                                                 | 102 ns: 1.02x faster                                                 |
| unpickle                 | 15.9 us                                                | 15.5 us: 1.02x faster                                                |
| async_tree_memoization   | 578 ms                                                 | 565 ms: 1.02x faster                                                 |
| sympy_integrate          | 21.4 ms                                                | 21.0 ms: 1.02x faster                                                |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 711 ms: 1.02x faster                                                 |
| unpickle_pure_python     | 230 us                                                 | 226 us: 1.02x faster                                                 |
| pickle_list              | 5.08 us                                                | 4.99 us: 1.02x faster                                                |
| create_gc_cycles         | 1.48 ms                                                | 1.46 ms: 1.01x faster                                                |
| dask                     | 372 ms                                                 | 367 ms: 1.01x faster                                                 |
| pickle_dict              | 35.5 us                                                | 35.1 us: 1.01x faster                                                |
| xml_etree_iterparse      | 107 ms                                                 | 106 ms: 1.01x faster                                                 |
| regex_effbot             | 3.61 ms                                                | 3.58 ms: 1.01x faster                                                |
| pickle                   | 11.6 us                                                | 11.5 us: 1.01x faster                                                |
| sqlglot_normalize        | 110 ms                                                 | 109 ms: 1.01x faster                                                 |
| sqlite_synth             | 2.83 us                                                | 2.82 us: 1.01x faster                                                |
| async_tree_none_tg       | 450 ms                                                 | 448 ms: 1.00x faster                                                 |
| bench_thread_pool        | 842 us                                                 | 840 us: 1.00x faster                                                 |
| mako                     | 11.9 ms                                                | 11.9 ms: 1.00x slower                                                |
| asyncio_tcp              | 491 ms                                                 | 493 ms: 1.00x slower                                                 |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                               |
| async_tree_io_tg         | 1.18 sec                                               | 1.19 sec: 1.01x slower                                               |
| richards_super           | 51.5 ms                                                | 52.0 ms: 1.01x slower                                                |
| sympy_expand             | 478 ms                                                 | 483 ms: 1.01x slower                                                 |
| json_dumps               | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                |
| async_generators         | 463 ms                                                 | 470 ms: 1.02x slower                                                 |
| deltablue                | 3.72 ms                                                | 3.78 ms: 1.02x slower                                                |
| async_tree_io            | 1.16 sec                                               | 1.18 sec: 1.02x slower                                               |
| sqlglot_optimize         | 54.8 ms                                                | 55.9 ms: 1.02x slower                                                |
| chaos                    | 67.0 ms                                                | 68.4 ms: 1.02x slower                                                |
| scimark_sor              | 129 ms                                                 | 133 ms: 1.03x slower                                                 |
| pycparser                | 1.18 sec                                               | 1.22 sec: 1.03x slower                                               |
| nqueens                  | 83.3 ms                                                | 87.0 ms: 1.04x slower                                                |
| pprint_safe_repr         | 776 ms                                                 | 812 ms: 1.05x slower                                                 |
| mdp                      | 2.63 sec                                               | 2.77 sec: 1.05x slower                                               |
| regex_dna                | 212 ms                                                 | 224 ms: 1.05x slower                                                 |
| python_startup           | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                |
| pprint_pformat           | 1.57 sec                                               | 1.69 sec: 1.08x slower                                               |
| go                       | 139 ms                                                 | 150 ms: 1.08x slower                                                 |
| spectral_norm            | 115 ms                                                 | 126 ms: 1.10x slower                                                 |
| regex_v8                 | 23.1 ms                                                | 25.6 ms: 1.11x slower                                                |
| telco                    | 7.10 ms                                                | 8.44 ms: 1.19x slower                                                |
| hexiom                   | 6.41 ms                                                | 7.81 ms: 1.22x slower                                                |
| python_startup_no_site   | 6.94 ms                                                | 8.77 ms: 1.26x slower                                                |
| coverage                 | 72.7 ms                                                | 94.5 ms: 1.30x slower                                                |
| Geometric mean           | (ref)                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (13): fannkuch, json, async_tree_cpu_io_mixed_tg, json_loads, dulwich_log, bench_mp_pool, pidigits, asyncio_websockets, 2to3, pyflate, richards, async_tree_memoization_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 89.80% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.96x