
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_continue
- machine: linux-x86_64
- commit hash: 9e86002
- commit date: 2024-02-13
- overall geometric mean: 1.02x faster \*
- HPT reliability: 99.84%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 273 ms: 1.00x faster                                                    |
| chameleon      | 7.41 ms                                                | 6.74 ms: 1.10x faster                                                   |
| docutils       | 2.77 sec                                               | 2.62 sec: 1.06x faster                                                  |
| tornado_http   | 103 ms                                                 | 96.7 ms: 1.06x faster                                                   |
| Geometric mean | (ref)                                                  | 1.05x faster                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 438 ms: 1.08x faster                                                    |
| async_tree_memoization  | 578 ms                                                 | 563 ms: 1.03x faster                                                    |
| async_tree_cpu_io_mixed | 726 ms                                                 | 708 ms: 1.02x faster                                                    |
| async_tree_none_tg      | 450 ms                                                 | 448 ms: 1.00x faster                                                    |
| async_tree_io_tg        | 1.18 sec                                               | 1.19 sec: 1.00x slower                                                  |
| async_tree_io           | 1.16 sec                                               | 1.17 sec: 1.01x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.02x faster                                                            |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 84.2 ms: 1.01x faster                                                   |
| nbody          | 97.0 ms                                                | 99.1 ms: 1.02x slower                                                   |
| Geometric mean | (ref)                                                  | 1.00x slower                                                            |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 136 ms: 1.09x faster                                                    |
| regex_effbot   | 3.61 ms                                                | 3.68 ms: 1.02x slower                                                   |
| regex_dna      | 212 ms                                                 | 224 ms: 1.05x slower                                                    |
| regex_v8       | 23.1 ms                                                | 25.6 ms: 1.11x slower                                                   |
| Geometric mean | (ref)                                                  | 1.02x slower                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 293 us: 1.10x faster                                                    |
| tomli_loads          | 2.33 sec                                               | 2.14 sec: 1.09x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 57.3 ms: 1.08x faster                                                   |
| pickle_dict          | 35.5 us                                                | 33.2 us: 1.07x faster                                                   |
| unpickle             | 15.9 us                                                | 15.0 us: 1.06x faster                                                   |
| xml_etree_generate   | 89.2 ms                                                | 84.8 ms: 1.05x faster                                                   |
| unpickle_list        | 5.29 us                                                | 5.04 us: 1.05x faster                                                   |
| pickle_list          | 5.08 us                                                | 4.91 us: 1.04x faster                                                   |
| json_loads           | 28.5 us                                                | 27.5 us: 1.04x faster                                                   |
| unpickle_pure_python | 230 us                                                 | 223 us: 1.03x faster                                                    |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                                    |
| pickle               | 11.6 us                                                | 11.4 us: 1.02x faster                                                   |
| json_dumps           | 10.4 ms                                                | 10.4 ms: 1.00x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                            |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                   |
| python_startup_no_site | 6.94 ms                                                | 8.83 ms: 1.27x slower                                                   |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|-----------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 12.0 ms: 1.01x slower                                                   |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|--------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 108 us: 1.46x faster                                                    |
| comprehensions           | 21.8 us                                                | 18.7 us: 1.16x faster                                                   |
| logging_format           | 7.23 us                                                | 6.34 us: 1.14x faster                                                   |
| raytrace                 | 312 ms                                                 | 276 ms: 1.13x faster                                                    |
| logging_simple           | 6.46 us                                                | 5.71 us: 1.13x faster                                                   |
| deltablue                | 3.72 ms                                                | 3.33 ms: 1.12x faster                                                   |
| deepcopy_reduce          | 3.35 us                                                | 3.03 us: 1.11x faster                                                   |
| pickle_pure_python       | 324 us                                                 | 293 us: 1.10x faster                                                    |
| chameleon                | 7.41 ms                                                | 6.74 ms: 1.10x faster                                                   |
| gc_traversal             | 3.79 ms                                                | 3.47 ms: 1.09x faster                                                   |
| deepcopy                 | 371 us                                                 | 340 us: 1.09x faster                                                    |
| deepcopy_memo            | 40.7 us                                                | 37.3 us: 1.09x faster                                                   |
| regex_compile            | 148 ms                                                 | 136 ms: 1.09x faster                                                    |
| tomli_loads              | 2.33 sec                                               | 2.14 sec: 1.09x faster                                                  |
| async_tree_none          | 472 ms                                                 | 438 ms: 1.08x faster                                                    |
| xml_etree_process        | 61.7 ms                                                | 57.3 ms: 1.08x faster                                                   |
| sympy_sum                | 169 ms                                                 | 157 ms: 1.08x faster                                                    |
| unpack_sequence          | 54.0 ns                                                | 50.2 ns: 1.08x faster                                                   |
| sympy_str                | 300 ms                                                 | 279 ms: 1.07x faster                                                    |
| sqlglot_parse            | 1.36 ms                                                | 1.27 ms: 1.07x faster                                                   |
| pickle_dict              | 35.5 us                                                | 33.2 us: 1.07x faster                                                   |
| tornado_http             | 103 ms                                                 | 96.7 ms: 1.06x faster                                                   |
| docutils                 | 2.77 sec                                               | 2.62 sec: 1.06x faster                                                  |
| unpickle                 | 15.9 us                                                | 15.0 us: 1.06x faster                                                   |
| generators               | 31.2 ms                                                | 29.6 ms: 1.05x faster                                                   |
| crypto_pyaes             | 81.9 ms                                                | 77.7 ms: 1.05x faster                                                   |
| xml_etree_generate       | 89.2 ms                                                | 84.8 ms: 1.05x faster                                                   |
| logging_silent           | 104 ns                                                 | 99.4 ns: 1.05x faster                                                   |
| sqlglot_transpile        | 1.68 ms                                                | 1.60 ms: 1.05x faster                                                   |
| unpickle_list            | 5.29 us                                                | 5.04 us: 1.05x faster                                                   |
| scimark_lu               | 118 ms                                                 | 113 ms: 1.04x faster                                                    |
| pathlib                  | 19.3 ms                                                | 18.5 ms: 1.04x faster                                                   |
| scimark_monte_carlo      | 75.1 ms                                                | 72.4 ms: 1.04x faster                                                   |
| scimark_sor              | 129 ms                                                 | 124 ms: 1.04x faster                                                    |
| sympy_integrate          | 21.4 ms                                                | 20.7 ms: 1.04x faster                                                   |
| pickle_list              | 5.08 us                                                | 4.91 us: 1.04x faster                                                   |
| json_loads               | 28.5 us                                                | 27.5 us: 1.04x faster                                                   |
| scimark_fft              | 382 ms                                                 | 370 ms: 1.03x faster                                                    |
| pprint_safe_repr         | 776 ms                                                 | 752 ms: 1.03x faster                                                    |
| json                     | 5.26 ms                                                | 5.10 ms: 1.03x faster                                                   |
| unpickle_pure_python     | 230 us                                                 | 223 us: 1.03x faster                                                    |
| dask                     | 372 ms                                                 | 361 ms: 1.03x faster                                                    |
| async_tree_memoization   | 578 ms                                                 | 563 ms: 1.03x faster                                                    |
| meteor_contest           | 112 ms                                                 | 110 ms: 1.02x faster                                                    |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 708 ms: 1.02x faster                                                    |
| richards                 | 45.8 ms                                                | 44.8 ms: 1.02x faster                                                   |
| coroutines               | 23.2 ms                                                | 22.6 ms: 1.02x faster                                                   |
| mdp                      | 2.63 sec                                               | 2.57 sec: 1.02x faster                                                  |
| sqlglot_normalize        | 110 ms                                                 | 108 ms: 1.02x faster                                                    |
| sqlite_synth             | 2.83 us                                                | 2.78 us: 1.02x faster                                                   |
| xml_etree_parse          | 159 ms                                                 | 156 ms: 1.02x faster                                                    |
| richards_super           | 51.5 ms                                                | 50.6 ms: 1.02x faster                                                   |
| dulwich_log              | 68.5 ms                                                | 67.3 ms: 1.02x faster                                                   |
| pickle                   | 11.6 us                                                | 11.4 us: 1.02x faster                                                   |
| sympy_expand             | 478 ms                                                 | 471 ms: 1.01x faster                                                    |
| pprint_pformat           | 1.57 sec                                               | 1.55 sec: 1.01x faster                                                  |
| create_gc_cycles         | 1.48 ms                                                | 1.46 ms: 1.01x faster                                                   |
| float                    | 84.7 ms                                                | 84.2 ms: 1.01x faster                                                   |
| bench_thread_pool        | 842 us                                                 | 836 us: 1.01x faster                                                    |
| async_tree_none_tg       | 450 ms                                                 | 448 ms: 1.00x faster                                                    |
| 2to3                     | 274 ms                                                 | 273 ms: 1.00x faster                                                    |
| asyncio_tcp              | 491 ms                                                 | 492 ms: 1.00x slower                                                    |
| async_tree_io_tg         | 1.18 sec                                               | 1.19 sec: 1.00x slower                                                  |
| json_dumps               | 10.4 ms                                                | 10.4 ms: 1.00x slower                                                   |
| fannkuch                 | 417 ms                                                 | 420 ms: 1.01x slower                                                    |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                  |
| mako                     | 11.9 ms                                                | 12.0 ms: 1.01x slower                                                   |
| async_tree_io            | 1.16 sec                                               | 1.17 sec: 1.01x slower                                                  |
| chaos                    | 67.0 ms                                                | 67.8 ms: 1.01x slower                                                   |
| regex_effbot             | 3.61 ms                                                | 3.68 ms: 1.02x slower                                                   |
| nbody                    | 97.0 ms                                                | 99.1 ms: 1.02x slower                                                   |
| pycparser                | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                  |
| pyflate                  | 482 ms                                                 | 496 ms: 1.03x slower                                                    |
| go                       | 139 ms                                                 | 146 ms: 1.05x slower                                                    |
| nqueens                  | 83.3 ms                                                | 87.8 ms: 1.05x slower                                                   |
| regex_dna                | 212 ms                                                 | 224 ms: 1.05x slower                                                    |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 5.34 ms: 1.06x slower                                                   |
| python_startup           | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                   |
| regex_v8                 | 23.1 ms                                                | 25.6 ms: 1.11x slower                                                   |
| spectral_norm            | 115 ms                                                 | 131 ms: 1.14x slower                                                    |
| hexiom                   | 6.41 ms                                                | 7.52 ms: 1.17x slower                                                   |
| telco                    | 7.10 ms                                                | 8.52 ms: 1.20x slower                                                   |
| python_startup_no_site   | 6.94 ms                                                | 8.83 ms: 1.27x slower                                                   |
| coverage                 | 72.7 ms                                                | 94.0 ms: 1.29x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.02x faster                                                            |

Benchmark hidden because not significant (9): async_tree_cpu_io_mixed_tg, xml_etree_iterparse, async_generators, async_tree_memoization_tg, sqlglot_optimize, bench_mp_pool, pidigits, asyncio_websockets, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.84% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.96x