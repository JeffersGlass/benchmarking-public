
# Results vs. 3.12.0

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: linux-x86_64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.02x slower
- HPT reliability: 99.98%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 281 ms: 1.03x slower                                                   |
| chameleon      | 7.41 ms                                                | 7.32 ms: 1.01x faster                                                  |
| docutils       | 2.77 sec                                               | 2.71 sec: 1.02x faster                                                 |
| tornado_http   | 103 ms                                                 | 98.2 ms: 1.05x faster                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 451 ms: 1.05x faster                                                   |
| async_tree_none_tg         | 450 ms                                                 | 454 ms: 1.01x slower                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 736 ms: 1.01x slower                                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 592 ms: 1.03x slower                                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                 |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.05x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 88.3 ms: 1.04x slower                                                  |
| pidigits       | 187 ms                                                 | 196 ms: 1.04x slower                                                   |
| nbody          | 97.0 ms                                                | 113 ms: 1.17x slower                                                   |
| Geometric mean | (ref)                                                  | 1.08x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 212 ms                                                 | 216 ms: 1.02x slower                                                   |
| regex_compile  | 148 ms                                                 | 151 ms: 1.02x slower                                                   |
| regex_v8       | 23.1 ms                                                | 26.1 ms: 1.13x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 303 us: 1.07x faster                                                   |
| unpickle             | 15.9 us                                                | 14.9 us: 1.07x faster                                                  |
| pickle_dict          | 35.5 us                                                | 34.0 us: 1.04x faster                                                  |
| json_loads           | 28.5 us                                                | 27.7 us: 1.03x faster                                                  |
| pickle               | 11.6 us                                                | 11.3 us: 1.03x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.02x faster                                                   |
| pickle_list          | 5.08 us                                                | 5.03 us: 1.01x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 61.2 ms: 1.01x faster                                                  |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                  |
| unpickle_pure_python | 230 us                                                 | 233 us: 1.02x slower                                                   |
| xml_etree_iterparse  | 107 ms                                                 | 109 ms: 1.02x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (3): tomli_loads, unpickle_list, xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.74 ms: 1.26x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 13.5 ms: 1.14x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 115 us: 1.37x faster                                                   |
| unpack_sequence            | 54.0 ns                                                | 44.3 ns: 1.22x faster                                                  |
| logging_simple             | 6.46 us                                                | 6.02 us: 1.07x faster                                                  |
| pickle_pure_python         | 324 us                                                 | 303 us: 1.07x faster                                                   |
| unpickle                   | 15.9 us                                                | 14.9 us: 1.07x faster                                                  |
| deepcopy_reduce            | 3.35 us                                                | 3.15 us: 1.06x faster                                                  |
| logging_format             | 7.23 us                                                | 6.81 us: 1.06x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.06x faster                                                   |
| comprehensions             | 21.8 us                                                | 20.7 us: 1.05x faster                                                  |
| raytrace                   | 312 ms                                                 | 297 ms: 1.05x faster                                                   |
| generators                 | 31.2 ms                                                | 29.8 ms: 1.05x faster                                                  |
| deepcopy                   | 371 us                                                 | 354 us: 1.05x faster                                                   |
| async_tree_none            | 472 ms                                                 | 451 ms: 1.05x faster                                                   |
| tornado_http               | 103 ms                                                 | 98.2 ms: 1.05x faster                                                  |
| pickle_dict                | 35.5 us                                                | 34.0 us: 1.04x faster                                                  |
| scimark_sor                | 129 ms                                                 | 124 ms: 1.04x faster                                                   |
| pathlib                    | 19.3 ms                                                | 18.7 ms: 1.04x faster                                                  |
| sympy_str                  | 300 ms                                                 | 290 ms: 1.03x faster                                                   |
| json_loads                 | 28.5 us                                                | 27.7 us: 1.03x faster                                                  |
| pickle                     | 11.6 us                                                | 11.3 us: 1.03x faster                                                  |
| coroutines                 | 23.2 ms                                                | 22.6 ms: 1.03x faster                                                  |
| sqlglot_parse              | 1.36 ms                                                | 1.33 ms: 1.03x faster                                                  |
| scimark_lu                 | 118 ms                                                 | 115 ms: 1.02x faster                                                   |
| docutils                   | 2.77 sec                                               | 2.71 sec: 1.02x faster                                                 |
| sqlglot_transpile          | 1.68 ms                                                | 1.66 ms: 1.02x faster                                                  |
| xml_etree_parse            | 159 ms                                                 | 157 ms: 1.02x faster                                                   |
| json                       | 5.26 ms                                                | 5.17 ms: 1.02x faster                                                  |
| deepcopy_memo              | 40.7 us                                                | 40.1 us: 1.02x faster                                                  |
| create_gc_cycles           | 1.48 ms                                                | 1.45 ms: 1.02x faster                                                  |
| chameleon                  | 7.41 ms                                                | 7.32 ms: 1.01x faster                                                  |
| sympy_integrate            | 21.4 ms                                                | 21.2 ms: 1.01x faster                                                  |
| pickle_list                | 5.08 us                                                | 5.03 us: 1.01x faster                                                  |
| dask                       | 372 ms                                                 | 368 ms: 1.01x faster                                                   |
| async_generators           | 463 ms                                                 | 458 ms: 1.01x faster                                                   |
| xml_etree_process          | 61.7 ms                                                | 61.2 ms: 1.01x faster                                                  |
| meteor_contest             | 112 ms                                                 | 112 ms: 1.00x faster                                                   |
| bench_thread_pool          | 842 us                                                 | 843 us: 1.00x slower                                                   |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                  |
| crypto_pyaes               | 81.9 ms                                                | 82.5 ms: 1.01x slower                                                  |
| asyncio_tcp                | 491 ms                                                 | 495 ms: 1.01x slower                                                   |
| dulwich_log                | 68.5 ms                                                | 69.1 ms: 1.01x slower                                                  |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                 |
| async_tree_none_tg         | 450 ms                                                 | 454 ms: 1.01x slower                                                   |
| sqlite_synth               | 2.83 us                                                | 2.87 us: 1.01x slower                                                  |
| mdp                        | 2.63 sec                                               | 2.67 sec: 1.01x slower                                                 |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 736 ms: 1.01x slower                                                   |
| unpickle_pure_python       | 230 us                                                 | 233 us: 1.02x slower                                                   |
| regex_dna                  | 212 ms                                                 | 216 ms: 1.02x slower                                                   |
| regex_compile              | 148 ms                                                 | 151 ms: 1.02x slower                                                   |
| fannkuch                   | 417 ms                                                 | 426 ms: 1.02x slower                                                   |
| xml_etree_iterparse        | 107 ms                                                 | 109 ms: 1.02x slower                                                   |
| sqlglot_normalize          | 110 ms                                                 | 113 ms: 1.02x slower                                                   |
| sympy_expand               | 478 ms                                                 | 490 ms: 1.03x slower                                                   |
| 2to3                       | 274 ms                                                 | 281 ms: 1.03x slower                                                   |
| pprint_safe_repr           | 776 ms                                                 | 798 ms: 1.03x slower                                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 592 ms: 1.03x slower                                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                 |
| logging_silent             | 104 ns                                                 | 108 ns: 1.03x slower                                                   |
| float                      | 84.7 ms                                                | 88.3 ms: 1.04x slower                                                  |
| pidigits                   | 187 ms                                                 | 196 ms: 1.04x slower                                                   |
| sqlglot_optimize           | 54.8 ms                                                | 57.4 ms: 1.05x slower                                                  |
| gc_traversal               | 3.79 ms                                                | 3.97 ms: 1.05x slower                                                  |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.05x slower                                                 |
| pyflate                    | 482 ms                                                 | 508 ms: 1.05x slower                                                   |
| richards                   | 45.8 ms                                                | 48.4 ms: 1.05x slower                                                  |
| python_startup             | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| pycparser                  | 1.18 sec                                               | 1.25 sec: 1.06x slower                                                 |
| scimark_monte_carlo        | 75.1 ms                                                | 79.7 ms: 1.06x slower                                                  |
| richards_super             | 51.5 ms                                                | 54.8 ms: 1.06x slower                                                  |
| pprint_pformat             | 1.57 sec                                               | 1.67 sec: 1.06x slower                                                 |
| chaos                      | 67.0 ms                                                | 71.7 ms: 1.07x slower                                                  |
| nqueens                    | 83.3 ms                                                | 91.3 ms: 1.10x slower                                                  |
| go                         | 139 ms                                                 | 155 ms: 1.11x slower                                                   |
| regex_v8                   | 23.1 ms                                                | 26.1 ms: 1.13x slower                                                  |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.72 ms: 1.13x slower                                                  |
| mako                       | 11.9 ms                                                | 13.5 ms: 1.14x slower                                                  |
| scimark_fft                | 382 ms                                                 | 443 ms: 1.16x slower                                                   |
| nbody                      | 97.0 ms                                                | 113 ms: 1.17x slower                                                   |
| spectral_norm              | 115 ms                                                 | 140 ms: 1.22x slower                                                   |
| deltablue                  | 3.72 ms                                                | 4.57 ms: 1.23x slower                                                  |
| telco                      | 7.10 ms                                                | 8.78 ms: 1.24x slower                                                  |
| python_startup_no_site     | 6.94 ms                                                | 8.74 ms: 1.26x slower                                                  |
| hexiom                     | 6.41 ms                                                | 8.15 ms: 1.27x slower                                                  |
| coverage                   | 72.7 ms                                                | 95.6 ms: 1.32x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                           |

Benchmark hidden because not significant (9): async_tree_cpu_io_mixed, tomli_loads, regex_effbot, unpickle_list, bench_mp_pool, async_tree_memoization, xml_etree_generate, asyncio_websockets, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.98% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.93x