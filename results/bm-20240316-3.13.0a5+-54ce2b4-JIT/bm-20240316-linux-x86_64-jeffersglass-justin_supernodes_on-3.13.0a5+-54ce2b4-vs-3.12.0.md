# Results vs. 3.12.0

- fork: jeffersglass
- ref: justin_supernodes_on
- machine: linux-x86_64
- commit hash: 54ce2b4
- commit date: 2024-03-16
- overall geometric mean: 1.09x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: 1.15x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 273 ms: 1.01x faster                                                         |
| chameleon      | 7.41 ms                                                | 6.76 ms: 1.10x faster                                                        |
| docutils       | 2.77 sec                                               | 2.38 sec: 1.16x faster                                                       |
| tornado_http   | 103 ms                                                 | 137 ms: 1.34x slower                                                         |
| Geometric mean | (ref)                                                  | 1.01x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 389 ms: 1.21x faster                                                         |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 606 ms: 1.20x faster                                                         |
| async_tree_memoization_tg  | 575 ms                                                 | 482 ms: 1.19x faster                                                         |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 611 ms: 1.19x faster                                                         |
| async_tree_none_tg         | 450 ms                                                 | 380 ms: 1.18x faster                                                         |
| async_tree_io_tg           | 1.18 sec                                               | 1.01 sec: 1.17x faster                                                       |
| async_tree_memoization     | 578 ms                                                 | 494 ms: 1.17x faster                                                         |
| async_tree_io              | 1.16 sec                                               | 1.04 sec: 1.11x faster                                                       |
| Geometric mean             | (ref)                                                  | 1.18x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 73.3 ms: 1.16x faster                                                        |
| pidigits       | 187 ms                                                 | 174 ms: 1.07x faster                                                         |
| nbody          | 97.0 ms                                                | 99.6 ms: 1.03x slower                                                        |
| Geometric mean | (ref)                                                  | 1.06x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 212 ms                                                 | 174 ms: 1.22x faster                                                         |
| regex_compile  | 148 ms                                                 | 125 ms: 1.18x faster                                                         |
| regex_effbot   | 3.61 ms                                                | 3.07 ms: 1.18x faster                                                        |
| Geometric mean | (ref)                                                  | 1.15x faster                                                                 |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_list          | 5.08 us                                                | 3.57 us: 1.42x faster                                                        |
| pickle_dict          | 35.5 us                                                | 26.2 us: 1.35x faster                                                        |
| pickle               | 11.6 us                                                | 8.98 us: 1.29x faster                                                        |
| json_loads           | 28.5 us                                                | 22.4 us: 1.27x faster                                                        |
| unpickle             | 15.9 us                                                | 12.5 us: 1.27x faster                                                        |
| tomli_loads          | 2.33 sec                                               | 1.85 sec: 1.26x faster                                                       |
| unpickle_list        | 5.29 us                                                | 4.22 us: 1.25x faster                                                        |
| xml_etree_iterparse  | 107 ms                                                 | 89.7 ms: 1.19x faster                                                        |
| xml_etree_parse      | 159 ms                                                 | 134 ms: 1.19x faster                                                         |
| json_dumps           | 10.4 ms                                                | 8.95 ms: 1.16x faster                                                        |
| xml_etree_generate   | 89.2 ms                                                | 79.0 ms: 1.13x faster                                                        |
| pickle_pure_python   | 324 us                                                 | 288 us: 1.13x faster                                                         |
| xml_etree_process    | 61.7 ms                                                | 55.3 ms: 1.12x faster                                                        |
| unpickle_pure_python | 230 us                                                 | 207 us: 1.11x faster                                                         |
| Geometric mean       | (ref)                                                  | 1.22x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 17.2 ms: 1.80x slower                                                        |
| python_startup_no_site | 6.94 ms                                                | 15.9 ms: 2.29x slower                                                        |
| Geometric mean         | (ref)                                                  | 2.03x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 9.10 ms: 1.31x faster                                                        |
| django_template | 34.6 ms                                                | 32.1 ms: 1.08x faster                                                        |
| Geometric mean  | (ref)                                                  | 1.19x faster                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| bench_mp_pool              | 24.0 ms                                                | 14.5 ms: 1.66x faster                                                        |
| typing_runtime_protocols   | 158 us                                                 | 103 us: 1.53x faster                                                         |
| create_gc_cycles           | 1.48 ms                                                | 1.02 ms: 1.45x faster                                                        |
| pickle_list                | 5.08 us                                                | 3.57 us: 1.42x faster                                                        |
| comprehensions             | 21.8 us                                                | 15.3 us: 1.42x faster                                                        |
| pickle_dict                | 35.5 us                                                | 26.2 us: 1.35x faster                                                        |
| crypto_pyaes               | 81.9 ms                                                | 61.9 ms: 1.32x faster                                                        |
| scimark_fft                | 382 ms                                                 | 289 ms: 1.32x faster                                                         |
| mako                       | 11.9 ms                                                | 9.10 ms: 1.31x faster                                                        |
| fannkuch                   | 417 ms                                                 | 321 ms: 1.30x faster                                                         |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 3.89 ms: 1.30x faster                                                        |
| pickle                     | 11.6 us                                                | 8.98 us: 1.29x faster                                                        |
| spectral_norm              | 115 ms                                                 | 89.6 ms: 1.28x faster                                                        |
| gc_traversal               | 3.79 ms                                                | 2.97 ms: 1.28x faster                                                        |
| json_loads                 | 28.5 us                                                | 22.4 us: 1.27x faster                                                        |
| unpickle                   | 15.9 us                                                | 12.5 us: 1.27x faster                                                        |
| async_generators           | 463 ms                                                 | 364 ms: 1.27x faster                                                         |
| tomli_loads                | 2.33 sec                                               | 1.85 sec: 1.26x faster                                                       |
| unpickle_list              | 5.29 us                                                | 4.22 us: 1.25x faster                                                        |
| deepcopy_memo              | 40.7 us                                                | 33.1 us: 1.23x faster                                                        |
| meteor_contest             | 112 ms                                                 | 91.5 ms: 1.23x faster                                                        |
| json                       | 5.26 ms                                                | 4.28 ms: 1.23x faster                                                        |
| regex_dna                  | 212 ms                                                 | 174 ms: 1.22x faster                                                         |
| sympy_sum                  | 169 ms                                                 | 139 ms: 1.22x faster                                                         |
| async_tree_none            | 472 ms                                                 | 389 ms: 1.21x faster                                                         |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 606 ms: 1.20x faster                                                         |
| sympy_str                  | 300 ms                                                 | 251 ms: 1.19x faster                                                         |
| async_tree_memoization_tg  | 575 ms                                                 | 482 ms: 1.19x faster                                                         |
| mdp                        | 2.63 sec                                               | 2.21 sec: 1.19x faster                                                       |
| xml_etree_iterparse        | 107 ms                                                 | 89.7 ms: 1.19x faster                                                        |
| xml_etree_parse            | 159 ms                                                 | 134 ms: 1.19x faster                                                         |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 611 ms: 1.19x faster                                                         |
| regex_compile              | 148 ms                                                 | 125 ms: 1.18x faster                                                         |
| async_tree_none_tg         | 450 ms                                                 | 380 ms: 1.18x faster                                                         |
| regex_effbot               | 3.61 ms                                                | 3.07 ms: 1.18x faster                                                        |
| deepcopy                   | 371 us                                                 | 316 us: 1.17x faster                                                         |
| async_tree_io_tg           | 1.18 sec                                               | 1.01 sec: 1.17x faster                                                       |
| async_tree_memoization     | 578 ms                                                 | 494 ms: 1.17x faster                                                         |
| docutils                   | 2.77 sec                                               | 2.38 sec: 1.16x faster                                                       |
| json_dumps                 | 10.4 ms                                                | 8.95 ms: 1.16x faster                                                        |
| logging_format             | 7.23 us                                                | 6.25 us: 1.16x faster                                                        |
| float                      | 84.7 ms                                                | 73.3 ms: 1.16x faster                                                        |
| deepcopy_reduce            | 3.35 us                                                | 2.93 us: 1.14x faster                                                        |
| raytrace                   | 312 ms                                                 | 273 ms: 1.14x faster                                                         |
| logging_simple             | 6.46 us                                                | 5.66 us: 1.14x faster                                                        |
| scimark_monte_carlo        | 75.1 ms                                                | 66.2 ms: 1.13x faster                                                        |
| chaos                      | 67.0 ms                                                | 59.2 ms: 1.13x faster                                                        |
| xml_etree_generate         | 89.2 ms                                                | 79.0 ms: 1.13x faster                                                        |
| pickle_pure_python         | 324 us                                                 | 288 us: 1.13x faster                                                         |
| sqlglot_transpile          | 1.68 ms                                                | 1.50 ms: 1.12x faster                                                        |
| sympy_expand               | 478 ms                                                 | 427 ms: 1.12x faster                                                         |
| sympy_integrate            | 21.4 ms                                                | 19.1 ms: 1.12x faster                                                        |
| xml_etree_process          | 61.7 ms                                                | 55.3 ms: 1.12x faster                                                        |
| sqlite_synth               | 2.83 us                                                | 2.54 us: 1.12x faster                                                        |
| async_tree_io              | 1.16 sec                                               | 1.04 sec: 1.11x faster                                                       |
| unpickle_pure_python       | 230 us                                                 | 207 us: 1.11x faster                                                         |
| pprint_safe_repr           | 776 ms                                                 | 697 ms: 1.11x faster                                                         |
| sqlglot_parse              | 1.36 ms                                                | 1.23 ms: 1.11x faster                                                        |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.61 sec: 1.11x faster                                                       |
| logging_silent             | 104 ns                                                 | 94.5 ns: 1.11x faster                                                        |
| generators                 | 31.2 ms                                                | 28.3 ms: 1.10x faster                                                        |
| pyflate                    | 482 ms                                                 | 439 ms: 1.10x faster                                                         |
| pprint_pformat             | 1.57 sec                                               | 1.43 sec: 1.10x faster                                                       |
| chameleon                  | 7.41 ms                                                | 6.76 ms: 1.10x faster                                                        |
| scimark_lu                 | 118 ms                                                 | 109 ms: 1.08x faster                                                         |
| django_template            | 34.6 ms                                                | 32.1 ms: 1.08x faster                                                        |
| hexiom                     | 6.41 ms                                                | 5.96 ms: 1.08x faster                                                        |
| pidigits                   | 187 ms                                                 | 174 ms: 1.07x faster                                                         |
| sqlglot_optimize           | 54.8 ms                                                | 51.7 ms: 1.06x faster                                                        |
| deltablue                  | 3.72 ms                                                | 3.51 ms: 1.06x faster                                                        |
| richards                   | 45.8 ms                                                | 44.3 ms: 1.04x faster                                                        |
| nqueens                    | 83.3 ms                                                | 81.4 ms: 1.02x faster                                                        |
| telco                      | 7.10 ms                                                | 7.00 ms: 1.01x faster                                                        |
| pycparser                  | 1.18 sec                                               | 1.16 sec: 1.01x faster                                                       |
| 2to3                       | 274 ms                                                 | 273 ms: 1.01x faster                                                         |
| coroutines                 | 23.2 ms                                                | 23.7 ms: 1.02x slower                                                        |
| nbody                      | 97.0 ms                                                | 99.6 ms: 1.03x slower                                                        |
| coverage                   | 72.7 ms                                                | 76.0 ms: 1.05x slower                                                        |
| asyncio_tcp                | 491 ms                                                 | 514 ms: 1.05x slower                                                         |
| go                         | 139 ms                                                 | 147 ms: 1.05x slower                                                         |
| dulwich_log                | 68.5 ms                                                | 73.5 ms: 1.07x slower                                                        |
| scimark_sor                | 129 ms                                                 | 140 ms: 1.08x slower                                                         |
| pathlib                    | 19.3 ms                                                | 22.4 ms: 1.16x slower                                                        |
| dask                       | 372 ms                                                 | 441 ms: 1.19x slower                                                         |
| asyncio_websockets         | 551 ms                                                 | 669 ms: 1.21x slower                                                         |
| tornado_http               | 103 ms                                                 | 137 ms: 1.34x slower                                                         |
| bench_thread_pool          | 842 us                                                 | 1.41 ms: 1.67x slower                                                        |
| python_startup             | 9.55 ms                                                | 17.2 ms: 1.80x slower                                                        |
| unpack_sequence            | 54.0 ns                                                | 99.0 ns: 1.83x slower                                                        |
| python_startup_no_site     | 6.94 ms                                                | 15.9 ms: 2.29x slower                                                        |
| sqlglot_normalize          | 110 ms                                                 | 269 ms: 2.44x slower                                                         |
| Geometric mean             | (ref)                                                  | 1.09x faster                                                                 |

Benchmark hidden because not significant (3): mypy2, regex_v8, richards_super
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240316-3.13.0a5+-54ce2b4-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.10x
- 95% likely to have a speedup of 1.10x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: 1.15x