# Results vs. 3.12.0

- fork: jeffersglass
- ref: justin_supernodes_on
- machine: linux-x86_64
- commit hash: f486338
- commit date: 2024-03-16
- overall geometric mean: 1.02x faster
- HPT reliability: 98.56%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.15x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 299 ms: 1.09x slower                                                         |
| chameleon      | 7.41 ms                                                | 7.13 ms: 1.04x faster                                                        |
| docutils       | 2.77 sec                                               | 2.64 sec: 1.05x faster                                                       |
| tornado_http   | 103 ms                                                 | 144 ms: 1.41x slower                                                         |
| Geometric mean | (ref)                                                  | 1.09x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.18 sec                                               | 1.13 sec: 1.05x faster                                                       |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 699 ms: 1.04x faster                                                         |
| async_tree_none_tg         | 450 ms                                                 | 445 ms: 1.01x faster                                                         |
| async_tree_memoization_tg  | 575 ms                                                 | 584 ms: 1.02x slower                                                         |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.05x slower                                                       |
| async_tree_memoization     | 578 ms                                                 | 610 ms: 1.06x slower                                                         |
| Geometric mean             | (ref)                                                  | 1.00x slower                                                                 |

Benchmark hidden because not significant (2): async_tree_none, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 79.2 ms: 1.07x faster                                                        |
| pidigits       | 187 ms                                                 | 186 ms: 1.01x faster                                                         |
| nbody          | 97.0 ms                                                | 103 ms: 1.06x slower                                                         |
| Geometric mean | (ref)                                                  | 1.00x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 133 ms: 1.11x faster                                                         |
| regex_dna      | 212 ms                                                 | 197 ms: 1.08x faster                                                         |
| regex_effbot   | 3.61 ms                                                | 3.42 ms: 1.05x faster                                                        |
| regex_v8       | 23.1 ms                                                | 24.6 ms: 1.06x slower                                                        |
| Geometric mean | (ref)                                                  | 1.04x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_list          | 5.08 us                                                | 3.76 us: 1.35x faster                                                        |
| pickle_dict          | 35.5 us                                                | 27.5 us: 1.29x faster                                                        |
| tomli_loads          | 2.33 sec                                               | 1.93 sec: 1.21x faster                                                       |
| pickle               | 11.6 us                                                | 9.69 us: 1.20x faster                                                        |
| unpickle             | 15.9 us                                                | 13.3 us: 1.19x faster                                                        |
| json_loads           | 28.5 us                                                | 24.1 us: 1.18x faster                                                        |
| unpickle_list        | 5.29 us                                                | 4.49 us: 1.18x faster                                                        |
| xml_etree_iterparse  | 107 ms                                                 | 97.9 ms: 1.09x faster                                                        |
| json_dumps           | 10.4 ms                                                | 9.63 ms: 1.08x faster                                                        |
| xml_etree_generate   | 89.2 ms                                                | 84.1 ms: 1.06x faster                                                        |
| xml_etree_process    | 61.7 ms                                                | 58.6 ms: 1.05x faster                                                        |
| xml_etree_parse      | 159 ms                                                 | 152 ms: 1.05x faster                                                         |
| pickle_pure_python   | 324 us                                                 | 312 us: 1.04x faster                                                         |
| unpickle_pure_python | 230 us                                                 | 223 us: 1.03x faster                                                         |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 18.3 ms: 1.92x slower                                                        |
| python_startup_no_site | 6.94 ms                                                | 16.8 ms: 2.42x slower                                                        |
| Geometric mean         | (ref)                                                  | 2.16x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako           | 11.9 ms                                                | 9.84 ms: 1.21x faster                                                        |
| Geometric mean | (ref)                                                  | 1.10x faster                                                                 |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| bench_mp_pool              | 24.0 ms                                                | 15.6 ms: 1.54x faster                                                        |
| typing_runtime_protocols   | 158 us                                                 | 106 us: 1.49x faster                                                         |
| pickle_list                | 5.08 us                                                | 3.76 us: 1.35x faster                                                        |
| create_gc_cycles           | 1.48 ms                                                | 1.10 ms: 1.34x faster                                                        |
| comprehensions             | 21.8 us                                                | 16.5 us: 1.32x faster                                                        |
| pickle_dict                | 35.5 us                                                | 27.5 us: 1.29x faster                                                        |
| scimark_fft                | 382 ms                                                 | 304 ms: 1.26x faster                                                         |
| spectral_norm              | 115 ms                                                 | 91.5 ms: 1.26x faster                                                        |
| crypto_pyaes               | 81.9 ms                                                | 65.4 ms: 1.25x faster                                                        |
| mako                       | 11.9 ms                                                | 9.84 ms: 1.21x faster                                                        |
| tomli_loads                | 2.33 sec                                               | 1.93 sec: 1.21x faster                                                       |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.21 ms: 1.20x faster                                                        |
| pickle                     | 11.6 us                                                | 9.69 us: 1.20x faster                                                        |
| fannkuch                   | 417 ms                                                 | 349 ms: 1.20x faster                                                         |
| unpickle                   | 15.9 us                                                | 13.3 us: 1.19x faster                                                        |
| json_loads                 | 28.5 us                                                | 24.1 us: 1.18x faster                                                        |
| unpickle_list              | 5.29 us                                                | 4.49 us: 1.18x faster                                                        |
| async_generators           | 463 ms                                                 | 400 ms: 1.16x faster                                                         |
| json                       | 5.26 ms                                                | 4.60 ms: 1.14x faster                                                        |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                                         |
| raytrace                   | 312 ms                                                 | 280 ms: 1.12x faster                                                         |
| sympy_str                  | 300 ms                                                 | 269 ms: 1.11x faster                                                         |
| meteor_contest             | 112 ms                                                 | 101 ms: 1.11x faster                                                         |
| regex_compile              | 148 ms                                                 | 133 ms: 1.11x faster                                                         |
| deepcopy_memo              | 40.7 us                                                | 36.6 us: 1.11x faster                                                        |
| mdp                        | 2.63 sec                                               | 2.39 sec: 1.10x faster                                                       |
| scimark_monte_carlo        | 75.1 ms                                                | 68.5 ms: 1.10x faster                                                        |
| chaos                      | 67.0 ms                                                | 61.3 ms: 1.09x faster                                                        |
| logging_format             | 7.23 us                                                | 6.62 us: 1.09x faster                                                        |
| xml_etree_iterparse        | 107 ms                                                 | 97.9 ms: 1.09x faster                                                        |
| deepcopy                   | 371 us                                                 | 343 us: 1.08x faster                                                         |
| json_dumps                 | 10.4 ms                                                | 9.63 ms: 1.08x faster                                                        |
| regex_dna                  | 212 ms                                                 | 197 ms: 1.08x faster                                                         |
| pyflate                    | 482 ms                                                 | 449 ms: 1.07x faster                                                         |
| logging_simple             | 6.46 us                                                | 6.03 us: 1.07x faster                                                        |
| float                      | 84.7 ms                                                | 79.2 ms: 1.07x faster                                                        |
| deepcopy_reduce            | 3.35 us                                                | 3.14 us: 1.07x faster                                                        |
| sqlite_synth               | 2.83 us                                                | 2.66 us: 1.06x faster                                                        |
| xml_etree_generate         | 89.2 ms                                                | 84.1 ms: 1.06x faster                                                        |
| regex_effbot               | 3.61 ms                                                | 3.42 ms: 1.05x faster                                                        |
| xml_etree_process          | 61.7 ms                                                | 58.6 ms: 1.05x faster                                                        |
| async_tree_io_tg           | 1.18 sec                                               | 1.13 sec: 1.05x faster                                                       |
| xml_etree_parse            | 159 ms                                                 | 152 ms: 1.05x faster                                                         |
| sqlglot_parse              | 1.36 ms                                                | 1.30 ms: 1.05x faster                                                        |
| docutils                   | 2.77 sec                                               | 2.64 sec: 1.05x faster                                                       |
| sympy_expand               | 478 ms                                                 | 457 ms: 1.05x faster                                                         |
| sympy_integrate            | 21.4 ms                                                | 20.6 ms: 1.04x faster                                                        |
| sqlglot_transpile          | 1.68 ms                                                | 1.62 ms: 1.04x faster                                                        |
| chameleon                  | 7.41 ms                                                | 7.13 ms: 1.04x faster                                                        |
| pickle_pure_python         | 324 us                                                 | 312 us: 1.04x faster                                                         |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 699 ms: 1.04x faster                                                         |
| pprint_safe_repr           | 776 ms                                                 | 750 ms: 1.03x faster                                                         |
| gc_traversal               | 3.79 ms                                                | 3.68 ms: 1.03x faster                                                        |
| unpickle_pure_python       | 230 us                                                 | 223 us: 1.03x faster                                                         |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.74 sec: 1.03x faster                                                       |
| hexiom                     | 6.41 ms                                                | 6.24 ms: 1.03x faster                                                        |
| logging_silent             | 104 ns                                                 | 102 ns: 1.03x faster                                                         |
| sqlglot_normalize          | 110 ms                                                 | 108 ms: 1.02x faster                                                         |
| pprint_pformat             | 1.57 sec                                               | 1.55 sec: 1.02x faster                                                       |
| async_tree_none_tg         | 450 ms                                                 | 445 ms: 1.01x faster                                                         |
| pidigits                   | 187 ms                                                 | 186 ms: 1.01x faster                                                         |
| scimark_lu                 | 118 ms                                                 | 119 ms: 1.01x slower                                                         |
| generators                 | 31.2 ms                                                | 31.6 ms: 1.01x slower                                                        |
| async_tree_memoization_tg  | 575 ms                                                 | 584 ms: 1.02x slower                                                         |
| sqlglot_optimize           | 54.8 ms                                                | 55.8 ms: 1.02x slower                                                        |
| richards_super             | 51.5 ms                                                | 52.7 ms: 1.02x slower                                                        |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.05x slower                                                       |
| nqueens                    | 83.3 ms                                                | 87.6 ms: 1.05x slower                                                        |
| async_tree_memoization     | 578 ms                                                 | 610 ms: 1.06x slower                                                         |
| nbody                      | 97.0 ms                                                | 103 ms: 1.06x slower                                                         |
| regex_v8                   | 23.1 ms                                                | 24.6 ms: 1.06x slower                                                        |
| pycparser                  | 1.18 sec                                               | 1.26 sec: 1.07x slower                                                       |
| telco                      | 7.10 ms                                                | 7.66 ms: 1.08x slower                                                        |
| 2to3                       | 274 ms                                                 | 299 ms: 1.09x slower                                                         |
| coverage                   | 72.7 ms                                                | 81.5 ms: 1.12x slower                                                        |
| coroutines                 | 23.2 ms                                                | 26.2 ms: 1.13x slower                                                        |
| go                         | 139 ms                                                 | 159 ms: 1.14x slower                                                         |
| dulwich_log                | 68.5 ms                                                | 78.0 ms: 1.14x slower                                                        |
| scimark_sor                | 129 ms                                                 | 148 ms: 1.14x slower                                                         |
| asyncio_tcp                | 491 ms                                                 | 584 ms: 1.19x slower                                                         |
| pathlib                    | 19.3 ms                                                | 23.9 ms: 1.23x slower                                                        |
| dask                       | 372 ms                                                 | 472 ms: 1.27x slower                                                         |
| asyncio_websockets         | 551 ms                                                 | 721 ms: 1.31x slower                                                         |
| tornado_http               | 103 ms                                                 | 144 ms: 1.41x slower                                                         |
| bench_thread_pool          | 842 us                                                 | 1.49 ms: 1.77x slower                                                        |
| python_startup             | 9.55 ms                                                | 18.3 ms: 1.92x slower                                                        |
| unpack_sequence            | 54.0 ns                                                | 104 ns: 1.93x slower                                                         |
| python_startup_no_site     | 6.94 ms                                                | 16.8 ms: 2.42x slower                                                        |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                                 |

Benchmark hidden because not significant (6): async_tree_none, richards, django_template, async_tree_cpu_io_mixed, deltablue, mypy2
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240316-3.13.0a5+-f486338-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 98.56% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.15x