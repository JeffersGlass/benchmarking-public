# Results vs. 3.12.0

- fork: python
- ref: e2a3e4b7488aff6fdc70
- machine: linux-x86_64
- commit hash: e2a3e4b
- commit date: 2024-02-28
- overall geometric mean: 1.05x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 261 ms: 1.05x faster                                                   |
| chameleon      | 7.41 ms                                                | 6.82 ms: 1.09x faster                                                  |
| docutils       | 2.77 sec                                               | 2.56 sec: 1.08x faster                                                 |
| tornado_http   | 103 ms                                                 | 94.7 ms: 1.08x faster                                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 431 ms: 1.09x faster                                                   |
| async_tree_memoization     | 578 ms                                                 | 555 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 699 ms: 1.04x faster                                                   |
| async_tree_none_tg         | 450 ms                                                 | 442 ms: 1.02x faster                                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 566 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 715 ms: 1.01x faster                                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.19 sec: 1.00x slower                                                 |
| async_tree_io              | 1.16 sec                                               | 1.16 sec: 1.01x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 86.5 ms: 1.12x faster                                                  |
| float          | 84.7 ms                                                | 79.0 ms: 1.07x faster                                                  |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                                   |
| Geometric mean | (ref)                                                  | 1.06x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 131 ms: 1.14x faster                                                   |
| regex_dna      | 212 ms                                                 | 219 ms: 1.03x slower                                                   |
| regex_effbot   | 3.61 ms                                                | 3.73 ms: 1.03x slower                                                  |
| regex_v8       | 23.1 ms                                                | 24.8 ms: 1.07x slower                                                  |
| Geometric mean | (ref)                                                  | 1.00x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 292 us: 1.11x faster                                                   |
| unpickle_pure_python | 230 us                                                 | 212 us: 1.09x faster                                                   |
| tomli_loads          | 2.33 sec                                               | 2.15 sec: 1.09x faster                                                 |
| unpickle_list        | 5.29 us                                                | 4.92 us: 1.07x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 57.8 ms: 1.07x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 84.7 ms: 1.05x faster                                                  |
| json_loads           | 28.5 us                                                | 27.1 us: 1.05x faster                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 104 ms: 1.03x faster                                                   |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.03x faster                                                   |
| pickle_dict          | 35.5 us                                                | 35.1 us: 1.01x faster                                                  |
| json_dumps           | 10.4 ms                                                | 10.3 ms: 1.00x faster                                                  |
| pickle               | 11.6 us                                                | 11.7 us: 1.01x slower                                                  |
| pickle_list          | 5.08 us                                                | 5.29 us: 1.04x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                           |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.81 ms: 1.27x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.0 ms: 1.08x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 110 us: 1.43x faster                                                   |
| comprehensions             | 21.8 us                                                | 16.1 us: 1.35x faster                                                  |
| unpack_sequence            | 54.0 ns                                                | 42.5 ns: 1.27x faster                                                  |
| raytrace                   | 312 ms                                                 | 260 ms: 1.20x faster                                                   |
| deltablue                  | 3.72 ms                                                | 3.15 ms: 1.18x faster                                                  |
| crypto_pyaes               | 81.9 ms                                                | 69.9 ms: 1.17x faster                                                  |
| logging_format             | 7.23 us                                                | 6.24 us: 1.16x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                                   |
| logging_simple             | 6.46 us                                                | 5.64 us: 1.15x faster                                                  |
| regex_compile              | 148 ms                                                 | 131 ms: 1.14x faster                                                   |
| sympy_str                  | 300 ms                                                 | 266 ms: 1.13x faster                                                   |
| nbody                      | 97.0 ms                                                | 86.5 ms: 1.12x faster                                                  |
| chaos                      | 67.0 ms                                                | 59.8 ms: 1.12x faster                                                  |
| scimark_monte_carlo        | 75.1 ms                                                | 67.5 ms: 1.11x faster                                                  |
| fannkuch                   | 417 ms                                                 | 376 ms: 1.11x faster                                                   |
| pickle_pure_python         | 324 us                                                 | 292 us: 1.11x faster                                                   |
| sympy_integrate            | 21.4 ms                                                | 19.4 ms: 1.10x faster                                                  |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.60 ms: 1.10x faster                                                  |
| deepcopy_reduce            | 3.35 us                                                | 3.04 us: 1.10x faster                                                  |
| logging_silent             | 104 ns                                                 | 95.1 ns: 1.10x faster                                                  |
| async_tree_none            | 472 ms                                                 | 431 ms: 1.09x faster                                                   |
| sqlglot_parse              | 1.36 ms                                                | 1.24 ms: 1.09x faster                                                  |
| hexiom                     | 6.41 ms                                                | 5.86 ms: 1.09x faster                                                  |
| pyflate                    | 482 ms                                                 | 442 ms: 1.09x faster                                                   |
| unpickle_pure_python       | 230 us                                                 | 212 us: 1.09x faster                                                   |
| chameleon                  | 7.41 ms                                                | 6.82 ms: 1.09x faster                                                  |
| tomli_loads                | 2.33 sec                                               | 2.15 sec: 1.09x faster                                                 |
| deepcopy_memo              | 40.7 us                                                | 37.5 us: 1.09x faster                                                  |
| pprint_safe_repr           | 776 ms                                                 | 715 ms: 1.08x faster                                                   |
| tornado_http               | 103 ms                                                 | 94.7 ms: 1.08x faster                                                  |
| pathlib                    | 19.3 ms                                                | 17.9 ms: 1.08x faster                                                  |
| mako                       | 11.9 ms                                                | 11.0 ms: 1.08x faster                                                  |
| scimark_fft                | 382 ms                                                 | 353 ms: 1.08x faster                                                   |
| sqlglot_transpile          | 1.68 ms                                                | 1.56 ms: 1.08x faster                                                  |
| docutils                   | 2.77 sec                                               | 2.56 sec: 1.08x faster                                                 |
| scimark_sor                | 129 ms                                                 | 120 ms: 1.08x faster                                                   |
| unpickle_list              | 5.29 us                                                | 4.92 us: 1.07x faster                                                  |
| nqueens                    | 83.3 ms                                                | 77.5 ms: 1.07x faster                                                  |
| float                      | 84.7 ms                                                | 79.0 ms: 1.07x faster                                                  |
| meteor_contest             | 112 ms                                                 | 105 ms: 1.07x faster                                                   |
| xml_etree_process          | 61.7 ms                                                | 57.8 ms: 1.07x faster                                                  |
| deepcopy                   | 371 us                                                 | 347 us: 1.07x faster                                                   |
| pprint_pformat             | 1.57 sec                                               | 1.47 sec: 1.07x faster                                                 |
| generators                 | 31.2 ms                                                | 29.4 ms: 1.06x faster                                                  |
| json                       | 5.26 ms                                                | 4.96 ms: 1.06x faster                                                  |
| sympy_expand               | 478 ms                                                 | 452 ms: 1.06x faster                                                   |
| spectral_norm              | 115 ms                                                 | 109 ms: 1.06x faster                                                   |
| sqlglot_normalize          | 110 ms                                                 | 104 ms: 1.06x faster                                                   |
| dulwich_log                | 68.5 ms                                                | 65.0 ms: 1.05x faster                                                  |
| xml_etree_generate         | 89.2 ms                                                | 84.7 ms: 1.05x faster                                                  |
| json_loads                 | 28.5 us                                                | 27.1 us: 1.05x faster                                                  |
| 2to3                       | 274 ms                                                 | 261 ms: 1.05x faster                                                   |
| async_tree_memoization     | 578 ms                                                 | 555 ms: 1.04x faster                                                   |
| scimark_lu                 | 118 ms                                                 | 113 ms: 1.04x faster                                                   |
| coroutines                 | 23.2 ms                                                | 22.3 ms: 1.04x faster                                                  |
| async_generators           | 463 ms                                                 | 445 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 699 ms: 1.04x faster                                                   |
| sqlglot_optimize           | 54.8 ms                                                | 52.8 ms: 1.04x faster                                                  |
| bench_thread_pool          | 842 us                                                 | 814 us: 1.03x faster                                                   |
| go                         | 139 ms                                                 | 135 ms: 1.03x faster                                                   |
| pycparser                  | 1.18 sec                                               | 1.15 sec: 1.03x faster                                                 |
| xml_etree_iterparse        | 107 ms                                                 | 104 ms: 1.03x faster                                                   |
| xml_etree_parse            | 159 ms                                                 | 156 ms: 1.03x faster                                                   |
| asyncio_tcp                | 491 ms                                                 | 483 ms: 1.02x faster                                                   |
| async_tree_none_tg         | 450 ms                                                 | 442 ms: 1.02x faster                                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 566 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 715 ms: 1.01x faster                                                   |
| pickle_dict                | 35.5 us                                                | 35.1 us: 1.01x faster                                                  |
| json_dumps                 | 10.4 ms                                                | 10.3 ms: 1.00x faster                                                  |
| pidigits                   | 187 ms                                                 | 187 ms: 1.00x faster                                                   |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.79 sec: 1.00x slower                                                 |
| async_tree_io_tg           | 1.18 sec                                               | 1.19 sec: 1.00x slower                                                 |
| create_gc_cycles           | 1.48 ms                                                | 1.48 ms: 1.00x slower                                                  |
| async_tree_io              | 1.16 sec                                               | 1.16 sec: 1.01x slower                                                 |
| pickle                     | 11.6 us                                                | 11.7 us: 1.01x slower                                                  |
| asyncio_websockets         | 551 ms                                                 | 560 ms: 1.01x slower                                                   |
| mdp                        | 2.63 sec                                               | 2.68 sec: 1.02x slower                                                 |
| regex_dna                  | 212 ms                                                 | 219 ms: 1.03x slower                                                   |
| regex_effbot               | 3.61 ms                                                | 3.73 ms: 1.03x slower                                                  |
| richards                   | 45.8 ms                                                | 47.5 ms: 1.04x slower                                                  |
| pickle_list                | 5.08 us                                                | 5.29 us: 1.04x slower                                                  |
| richards_super             | 51.5 ms                                                | 53.8 ms: 1.04x slower                                                  |
| gc_traversal               | 3.79 ms                                                | 4.00 ms: 1.05x slower                                                  |
| python_startup             | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                  |
| regex_v8                   | 23.1 ms                                                | 24.8 ms: 1.07x slower                                                  |
| telco                      | 7.10 ms                                                | 8.34 ms: 1.17x slower                                                  |
| python_startup_no_site     | 6.94 ms                                                | 8.81 ms: 1.27x slower                                                  |
| coverage                   | 72.7 ms                                                | 95.2 ms: 1.31x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                           |

Benchmark hidden because not significant (4): unpickle, sqlite_synth, bench_mp_pool, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.93x