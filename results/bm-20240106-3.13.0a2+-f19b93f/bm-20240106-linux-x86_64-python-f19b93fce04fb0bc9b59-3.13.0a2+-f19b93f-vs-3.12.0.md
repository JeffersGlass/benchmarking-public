
# Results vs. 3.12.0

- fork: python
- ref: f19b93fce04fb0bc9b59
- machine: linux-x86_64
- commit hash: f19b93f
- commit date: 2024-01-06
- overall geometric mean: 1.04x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 263 ms: 1.04x faster                                                   |
| chameleon      | 7.41 ms                                                | 6.94 ms: 1.07x faster                                                  |
| docutils       | 2.77 sec                                               | 2.58 sec: 1.07x faster                                                 |
| tornado_http   | 103 ms                                                 | 94.2 ms: 1.09x faster                                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 431 ms: 1.09x faster                                                   |
| async_tree_memoization     | 578 ms                                                 | 557 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 703 ms: 1.03x faster                                                   |
| async_tree_none_tg         | 450 ms                                                 | 439 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 716 ms: 1.01x faster                                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                 |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (1): async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 86.9 ms: 1.12x faster                                                  |
| float          | 84.7 ms                                                | 80.0 ms: 1.06x faster                                                  |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x slower                                                   |
| Geometric mean | (ref)                                                  | 1.06x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 130 ms: 1.14x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.62 ms: 1.00x slower                                                  |
| regex_dna      | 212 ms                                                 | 218 ms: 1.03x slower                                                   |
| regex_v8       | 23.1 ms                                                | 24.9 ms: 1.08x slower                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.12 sec: 1.10x faster                                                 |
| pickle_pure_python   | 324 us                                                 | 299 us: 1.08x faster                                                   |
| unpickle_pure_python | 230 us                                                 | 214 us: 1.07x faster                                                   |
| xml_etree_process    | 61.7 ms                                                | 59.2 ms: 1.04x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 85.6 ms: 1.04x faster                                                  |
| unpickle             | 15.9 us                                                | 15.5 us: 1.02x faster                                                  |
| pickle_dict          | 35.5 us                                                | 34.9 us: 1.02x faster                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 105 ms: 1.01x faster                                                   |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.01x faster                                                   |
| pickle               | 11.6 us                                                | 11.5 us: 1.01x faster                                                  |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                  |
| unpickle_list        | 5.29 us                                                | 5.45 us: 1.03x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (2): json_loads, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.05x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.68 ms: 1.25x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.0 ms: 1.08x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 111 us: 1.42x faster                                                   |
| comprehensions             | 21.8 us                                                | 16.3 us: 1.34x faster                                                  |
| raytrace                   | 312 ms                                                 | 261 ms: 1.20x faster                                                   |
| logging_format             | 7.23 us                                                | 6.19 us: 1.17x faster                                                  |
| unpack_sequence            | 54.0 ns                                                | 46.5 ns: 1.16x faster                                                  |
| deltablue                  | 3.72 ms                                                | 3.20 ms: 1.16x faster                                                  |
| crypto_pyaes               | 81.9 ms                                                | 70.7 ms: 1.16x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                                   |
| logging_simple             | 6.46 us                                                | 5.63 us: 1.15x faster                                                  |
| regex_compile              | 148 ms                                                 | 130 ms: 1.14x faster                                                   |
| chaos                      | 67.0 ms                                                | 59.0 ms: 1.13x faster                                                  |
| sympy_str                  | 300 ms                                                 | 267 ms: 1.12x faster                                                   |
| nbody                      | 97.0 ms                                                | 86.9 ms: 1.12x faster                                                  |
| sympy_integrate            | 21.4 ms                                                | 19.3 ms: 1.11x faster                                                  |
| scimark_monte_carlo        | 75.1 ms                                                | 67.9 ms: 1.11x faster                                                  |
| tomli_loads                | 2.33 sec                                               | 2.12 sec: 1.10x faster                                                 |
| sqlglot_parse              | 1.36 ms                                                | 1.24 ms: 1.10x faster                                                  |
| async_tree_none            | 472 ms                                                 | 431 ms: 1.09x faster                                                   |
| tornado_http               | 103 ms                                                 | 94.2 ms: 1.09x faster                                                  |
| deepcopy_reduce            | 3.35 us                                                | 3.07 us: 1.09x faster                                                  |
| mako                       | 11.9 ms                                                | 11.0 ms: 1.08x faster                                                  |
| pickle_pure_python         | 324 us                                                 | 299 us: 1.08x faster                                                   |
| sqlglot_transpile          | 1.68 ms                                                | 1.56 ms: 1.08x faster                                                  |
| deepcopy_memo              | 40.7 us                                                | 37.9 us: 1.08x faster                                                  |
| gc_traversal               | 3.79 ms                                                | 3.53 ms: 1.07x faster                                                  |
| docutils                   | 2.77 sec                                               | 2.58 sec: 1.07x faster                                                 |
| unpickle_pure_python       | 230 us                                                 | 214 us: 1.07x faster                                                   |
| deepcopy                   | 371 us                                                 | 348 us: 1.07x faster                                                   |
| chameleon                  | 7.41 ms                                                | 6.94 ms: 1.07x faster                                                  |
| pathlib                    | 19.3 ms                                                | 18.1 ms: 1.07x faster                                                  |
| pprint_safe_repr           | 776 ms                                                 | 728 ms: 1.07x faster                                                   |
| generators                 | 31.2 ms                                                | 29.4 ms: 1.06x faster                                                  |
| scimark_fft                | 382 ms                                                 | 361 ms: 1.06x faster                                                   |
| float                      | 84.7 ms                                                | 80.0 ms: 1.06x faster                                                  |
| hexiom                     | 6.41 ms                                                | 6.07 ms: 1.06x faster                                                  |
| coroutines                 | 23.2 ms                                                | 22.0 ms: 1.06x faster                                                  |
| sympy_expand               | 478 ms                                                 | 454 ms: 1.05x faster                                                   |
| pprint_pformat             | 1.57 sec                                               | 1.49 sec: 1.05x faster                                                 |
| spectral_norm              | 115 ms                                                 | 109 ms: 1.05x faster                                                   |
| meteor_contest             | 112 ms                                                 | 107 ms: 1.05x faster                                                   |
| async_generators           | 463 ms                                                 | 443 ms: 1.05x faster                                                   |
| 2to3                       | 274 ms                                                 | 263 ms: 1.04x faster                                                   |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.85 ms: 1.04x faster                                                  |
| xml_etree_process          | 61.7 ms                                                | 59.2 ms: 1.04x faster                                                  |
| fannkuch                   | 417 ms                                                 | 400 ms: 1.04x faster                                                   |
| dulwich_log                | 68.5 ms                                                | 65.8 ms: 1.04x faster                                                  |
| xml_etree_generate         | 89.2 ms                                                | 85.6 ms: 1.04x faster                                                  |
| async_tree_memoization     | 578 ms                                                 | 557 ms: 1.04x faster                                                   |
| scimark_lu                 | 118 ms                                                 | 114 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 703 ms: 1.03x faster                                                   |
| mdp                        | 2.63 sec                                               | 2.55 sec: 1.03x faster                                                 |
| sqlglot_normalize          | 110 ms                                                 | 107 ms: 1.03x faster                                                   |
| asyncio_tcp                | 491 ms                                                 | 475 ms: 1.03x faster                                                   |
| dask                       | 372 ms                                                 | 360 ms: 1.03x faster                                                   |
| pyflate                    | 482 ms                                                 | 468 ms: 1.03x faster                                                   |
| async_tree_none_tg         | 450 ms                                                 | 439 ms: 1.02x faster                                                   |
| unpickle                   | 15.9 us                                                | 15.5 us: 1.02x faster                                                  |
| sqlglot_optimize           | 54.8 ms                                                | 53.7 ms: 1.02x faster                                                  |
| bench_thread_pool          | 842 us                                                 | 826 us: 1.02x faster                                                   |
| pickle_dict                | 35.5 us                                                | 34.9 us: 1.02x faster                                                  |
| xml_etree_iterparse        | 107 ms                                                 | 105 ms: 1.01x faster                                                   |
| xml_etree_parse            | 159 ms                                                 | 157 ms: 1.01x faster                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 716 ms: 1.01x faster                                                   |
| scimark_sor                | 129 ms                                                 | 128 ms: 1.01x faster                                                   |
| pickle                     | 11.6 us                                                | 11.5 us: 1.01x faster                                                  |
| create_gc_cycles           | 1.48 ms                                                | 1.47 ms: 1.01x faster                                                  |
| logging_silent             | 104 ns                                                 | 104 ns: 1.01x faster                                                   |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.78 sec: 1.00x faster                                                 |
| pidigits                   | 187 ms                                                 | 187 ms: 1.00x slower                                                   |
| regex_effbot               | 3.61 ms                                                | 3.62 ms: 1.00x slower                                                  |
| async_tree_io_tg           | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                 |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                  |
| pycparser                  | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                 |
| richards                   | 45.8 ms                                                | 46.9 ms: 1.02x slower                                                  |
| unpickle_list              | 5.29 us                                                | 5.45 us: 1.03x slower                                                  |
| regex_dna                  | 212 ms                                                 | 218 ms: 1.03x slower                                                   |
| richards_super             | 51.5 ms                                                | 53.6 ms: 1.04x slower                                                  |
| python_startup             | 9.55 ms                                                | 10.1 ms: 1.05x slower                                                  |
| regex_v8                   | 23.1 ms                                                | 24.9 ms: 1.08x slower                                                  |
| telco                      | 7.10 ms                                                | 8.26 ms: 1.16x slower                                                  |
| python_startup_no_site     | 6.94 ms                                                | 8.68 ms: 1.25x slower                                                  |
| coverage                   | 72.7 ms                                                | 96.4 ms: 1.33x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.04x faster                                                           |

Benchmark hidden because not significant (10): async_tree_memoization_tg, sqlite_synth, json, json_loads, go, nqueens, asyncio_websockets, bench_mp_pool, pickle_list, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.93x