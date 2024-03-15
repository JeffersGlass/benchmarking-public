
# Results vs. 3.12.0

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: linux-x86_64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.04x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 263 ms: 1.04x faster                                                   |
| chameleon      | 7.41 ms                                                | 6.94 ms: 1.07x faster                                                  |
| docutils       | 2.77 sec                                               | 2.64 sec: 1.05x faster                                                 |
| tornado_http   | 103 ms                                                 | 94.4 ms: 1.09x faster                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 434 ms: 1.09x faster                                                   |
| async_tree_memoization     | 578 ms                                                 | 557 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 703 ms: 1.03x faster                                                   |
| async_tree_none_tg         | 450 ms                                                 | 439 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 718 ms: 1.01x faster                                                   |
| async_tree_io              | 1.16 sec                                               | 1.17 sec: 1.01x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (2): async_tree_memoization_tg, async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 88.9 ms: 1.09x faster                                                  |
| float          | 84.7 ms                                                | 80.7 ms: 1.05x faster                                                  |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x slower                                                   |
| Geometric mean | (ref)                                                  | 1.05x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 129 ms: 1.15x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.58 ms: 1.01x faster                                                  |
| regex_v8       | 23.1 ms                                                | 23.5 ms: 1.02x slower                                                  |
| regex_dna      | 212 ms                                                 | 222 ms: 1.05x slower                                                   |
| Geometric mean | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 297 us: 1.09x faster                                                   |
| tomli_loads          | 2.33 sec                                               | 2.14 sec: 1.09x faster                                                 |
| unpickle             | 15.9 us                                                | 14.7 us: 1.08x faster                                                  |
| unpickle_pure_python | 230 us                                                 | 216 us: 1.07x faster                                                   |
| unpickle_list        | 5.29 us                                                | 5.02 us: 1.05x faster                                                  |
| pickle_dict          | 35.5 us                                                | 33.9 us: 1.05x faster                                                  |
| json_loads           | 28.5 us                                                | 27.5 us: 1.03x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 59.7 ms: 1.03x faster                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 104 ms: 1.02x faster                                                   |
| pickle               | 11.6 us                                                | 11.4 us: 1.01x faster                                                  |
| pickle_list          | 5.08 us                                                | 5.01 us: 1.01x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| xml_etree_generate   | 89.2 ms                                                | 88.2 ms: 1.01x faster                                                  |
| json_dumps           | 10.4 ms                                                | 10.3 ms: 1.01x faster                                                  |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.05x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.72 ms: 1.26x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.5 ms: 1.04x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 110 us: 1.44x faster                                                   |
| comprehensions             | 21.8 us                                                | 16.1 us: 1.35x faster                                                  |
| raytrace                   | 312 ms                                                 | 259 ms: 1.20x faster                                                   |
| deltablue                  | 3.72 ms                                                | 3.19 ms: 1.16x faster                                                  |
| unpack_sequence            | 54.0 ns                                                | 46.8 ns: 1.15x faster                                                  |
| logging_format             | 7.23 us                                                | 6.28 us: 1.15x faster                                                  |
| regex_compile              | 148 ms                                                 | 129 ms: 1.15x faster                                                   |
| crypto_pyaes               | 81.9 ms                                                | 71.7 ms: 1.14x faster                                                  |
| logging_simple             | 6.46 us                                                | 5.70 us: 1.13x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 149 ms: 1.13x faster                                                   |
| chaos                      | 67.0 ms                                                | 59.7 ms: 1.12x faster                                                  |
| sympy_str                  | 300 ms                                                 | 269 ms: 1.11x faster                                                   |
| scimark_monte_carlo        | 75.1 ms                                                | 68.0 ms: 1.11x faster                                                  |
| sympy_integrate            | 21.4 ms                                                | 19.5 ms: 1.10x faster                                                  |
| nbody                      | 97.0 ms                                                | 88.9 ms: 1.09x faster                                                  |
| pickle_pure_python         | 324 us                                                 | 297 us: 1.09x faster                                                   |
| generators                 | 31.2 ms                                                | 28.6 ms: 1.09x faster                                                  |
| sqlglot_parse              | 1.36 ms                                                | 1.25 ms: 1.09x faster                                                  |
| tomli_loads                | 2.33 sec                                               | 2.14 sec: 1.09x faster                                                 |
| tornado_http               | 103 ms                                                 | 94.4 ms: 1.09x faster                                                  |
| async_tree_none            | 472 ms                                                 | 434 ms: 1.09x faster                                                   |
| deepcopy_memo              | 40.7 us                                                | 37.6 us: 1.08x faster                                                  |
| unpickle                   | 15.9 us                                                | 14.7 us: 1.08x faster                                                  |
| scimark_sor                | 129 ms                                                 | 120 ms: 1.08x faster                                                   |
| pyflate                    | 482 ms                                                 | 448 ms: 1.08x faster                                                   |
| deepcopy_reduce            | 3.35 us                                                | 3.11 us: 1.08x faster                                                  |
| sqlglot_transpile          | 1.68 ms                                                | 1.57 ms: 1.07x faster                                                  |
| pathlib                    | 19.3 ms                                                | 18.1 ms: 1.07x faster                                                  |
| deepcopy                   | 371 us                                                 | 347 us: 1.07x faster                                                   |
| chameleon                  | 7.41 ms                                                | 6.94 ms: 1.07x faster                                                  |
| unpickle_pure_python       | 230 us                                                 | 216 us: 1.07x faster                                                   |
| pprint_safe_repr           | 776 ms                                                 | 729 ms: 1.06x faster                                                   |
| hexiom                     | 6.41 ms                                                | 6.05 ms: 1.06x faster                                                  |
| pprint_pformat             | 1.57 sec                                               | 1.48 sec: 1.06x faster                                                 |
| unpickle_list              | 5.29 us                                                | 5.02 us: 1.05x faster                                                  |
| float                      | 84.7 ms                                                | 80.7 ms: 1.05x faster                                                  |
| pickle_dict                | 35.5 us                                                | 33.9 us: 1.05x faster                                                  |
| docutils                   | 2.77 sec                                               | 2.64 sec: 1.05x faster                                                 |
| dulwich_log                | 68.5 ms                                                | 65.5 ms: 1.05x faster                                                  |
| sympy_expand               | 478 ms                                                 | 457 ms: 1.05x faster                                                   |
| 2to3                       | 274 ms                                                 | 263 ms: 1.04x faster                                                   |
| nqueens                    | 83.3 ms                                                | 79.8 ms: 1.04x faster                                                  |
| sqlglot_normalize          | 110 ms                                                 | 106 ms: 1.04x faster                                                   |
| scimark_fft                | 382 ms                                                 | 367 ms: 1.04x faster                                                   |
| json                       | 5.26 ms                                                | 5.05 ms: 1.04x faster                                                  |
| async_generators           | 463 ms                                                 | 444 ms: 1.04x faster                                                   |
| meteor_contest             | 112 ms                                                 | 108 ms: 1.04x faster                                                   |
| scimark_lu                 | 118 ms                                                 | 113 ms: 1.04x faster                                                   |
| mdp                        | 2.63 sec                                               | 2.53 sec: 1.04x faster                                                 |
| spectral_norm              | 115 ms                                                 | 111 ms: 1.04x faster                                                   |
| fannkuch                   | 417 ms                                                 | 402 ms: 1.04x faster                                                   |
| mako                       | 11.9 ms                                                | 11.5 ms: 1.04x faster                                                  |
| async_tree_memoization     | 578 ms                                                 | 557 ms: 1.04x faster                                                   |
| json_loads                 | 28.5 us                                                | 27.5 us: 1.03x faster                                                  |
| xml_etree_process          | 61.7 ms                                                | 59.7 ms: 1.03x faster                                                  |
| dask                       | 372 ms                                                 | 360 ms: 1.03x faster                                                   |
| gc_traversal               | 3.79 ms                                                | 3.67 ms: 1.03x faster                                                  |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 703 ms: 1.03x faster                                                   |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.92 ms: 1.03x faster                                                  |
| coroutines                 | 23.2 ms                                                | 22.6 ms: 1.03x faster                                                  |
| sqlglot_optimize           | 54.8 ms                                                | 53.5 ms: 1.03x faster                                                  |
| xml_etree_iterparse        | 107 ms                                                 | 104 ms: 1.02x faster                                                   |
| logging_silent             | 104 ns                                                 | 102 ns: 1.02x faster                                                   |
| async_tree_none_tg         | 450 ms                                                 | 439 ms: 1.02x faster                                                   |
| asyncio_tcp                | 491 ms                                                 | 482 ms: 1.02x faster                                                   |
| go                         | 139 ms                                                 | 137 ms: 1.02x faster                                                   |
| bench_thread_pool          | 842 us                                                 | 828 us: 1.02x faster                                                   |
| pickle                     | 11.6 us                                                | 11.4 us: 1.01x faster                                                  |
| pickle_list                | 5.08 us                                                | 5.01 us: 1.01x faster                                                  |
| xml_etree_parse            | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 718 ms: 1.01x faster                                                   |
| xml_etree_generate         | 89.2 ms                                                | 88.2 ms: 1.01x faster                                                  |
| regex_effbot               | 3.61 ms                                                | 3.58 ms: 1.01x faster                                                  |
| json_dumps                 | 10.4 ms                                                | 10.3 ms: 1.01x faster                                                  |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.78 sec: 1.00x faster                                                 |
| pidigits                   | 187 ms                                                 | 187 ms: 1.00x slower                                                   |
| async_tree_io              | 1.16 sec                                               | 1.17 sec: 1.01x slower                                                 |
| regex_v8                   | 23.1 ms                                                | 23.5 ms: 1.02x slower                                                  |
| pycparser                  | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| richards                   | 45.8 ms                                                | 47.4 ms: 1.03x slower                                                  |
| richards_super             | 51.5 ms                                                | 53.9 ms: 1.05x slower                                                  |
| regex_dna                  | 212 ms                                                 | 222 ms: 1.05x slower                                                   |
| python_startup             | 9.55 ms                                                | 10.1 ms: 1.05x slower                                                  |
| telco                      | 7.10 ms                                                | 8.35 ms: 1.18x slower                                                  |
| python_startup_no_site     | 6.94 ms                                                | 8.72 ms: 1.26x slower                                                  |
| coverage                   | 72.7 ms                                                | 96.8 ms: 1.33x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.04x faster                                                           |

Benchmark hidden because not significant (7): async_tree_memoization_tg, create_gc_cycles, asyncio_websockets, sqlite_synth, bench_mp_pool, async_tree_io_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.93x