# Results vs. 3.12.0

- fork: jeffersglass
- ref: justin_supernodes_on
- machine: linux-x86_64
- commit hash: 54ce2b4
- commit date: 2024-03-16
- overall geometric mean: 1.00x faster
- HPT reliability: 83.23%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.15x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 304 ms: 1.11x slower                                                         |
| tornado_http   | 103 ms                                                 | 145 ms: 1.41x slower                                                         |
| Geometric mean | (ref)                                                  | 1.12x slower                                                                 |

Benchmark hidden because not significant (2): chameleon, docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 682 ms: 1.06x faster                                                         |
| async_tree_io_tg           | 1.18 sec                                               | 1.14 sec: 1.03x faster                                                       |
| async_tree_none_tg         | 450 ms                                                 | 440 ms: 1.02x faster                                                         |
| async_tree_memoization_tg  | 575 ms                                                 | 590 ms: 1.03x slower                                                         |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.05x slower                                                       |
| async_tree_memoization     | 578 ms                                                 | 607 ms: 1.05x slower                                                         |
| Geometric mean             | (ref)                                                  | 1.00x slower                                                                 |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 79.8 ms: 1.06x faster                                                        |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                                         |
| nbody          | 97.0 ms                                                | 107 ms: 1.10x slower                                                         |
| Geometric mean | (ref)                                                  | 1.01x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 212 ms                                                 | 188 ms: 1.13x faster                                                         |
| regex_compile  | 148 ms                                                 | 134 ms: 1.11x faster                                                         |
| regex_effbot   | 3.61 ms                                                | 3.42 ms: 1.06x faster                                                        |
| regex_v8       | 23.1 ms                                                | 24.6 ms: 1.06x slower                                                        |
| Geometric mean | (ref)                                                  | 1.06x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_list          | 5.08 us                                                | 3.83 us: 1.33x faster                                                        |
| pickle_dict          | 35.5 us                                                | 28.7 us: 1.24x faster                                                        |
| json_loads           | 28.5 us                                                | 24.0 us: 1.19x faster                                                        |
| pickle               | 11.6 us                                                | 9.82 us: 1.18x faster                                                        |
| tomli_loads          | 2.33 sec                                               | 1.98 sec: 1.18x faster                                                       |
| unpickle             | 15.9 us                                                | 13.7 us: 1.16x faster                                                        |
| unpickle_list        | 5.29 us                                                | 4.56 us: 1.16x faster                                                        |
| json_dumps           | 10.4 ms                                                | 9.57 ms: 1.09x faster                                                        |
| xml_etree_parse      | 159 ms                                                 | 148 ms: 1.08x faster                                                         |
| xml_etree_iterparse  | 107 ms                                                 | 101 ms: 1.06x faster                                                         |
| pickle_pure_python   | 324 us                                                 | 308 us: 1.05x faster                                                         |
| xml_etree_generate   | 89.2 ms                                                | 85.2 ms: 1.05x faster                                                        |
| xml_etree_process    | 61.7 ms                                                | 59.3 ms: 1.04x faster                                                        |
| unpickle_pure_python | 230 us                                                 | 223 us: 1.03x faster                                                         |
| Geometric mean       | (ref)                                                  | 1.13x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 19.3 ms: 2.02x slower                                                        |
| python_startup_no_site | 6.94 ms                                                | 17.8 ms: 2.56x slower                                                        |
| Geometric mean         | (ref)                                                  | 2.27x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako           | 11.9 ms                                                | 10.1 ms: 1.17x faster                                                        |
| Geometric mean | (ref)                                                  | 1.08x faster                                                                 |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| bench_mp_pool              | 24.0 ms                                                | 16.2 ms: 1.49x faster                                                        |
| typing_runtime_protocols   | 158 us                                                 | 107 us: 1.48x faster                                                         |
| create_gc_cycles           | 1.48 ms                                                | 1.11 ms: 1.33x faster                                                        |
| pickle_list                | 5.08 us                                                | 3.83 us: 1.33x faster                                                        |
| comprehensions             | 21.8 us                                                | 16.7 us: 1.30x faster                                                        |
| spectral_norm              | 115 ms                                                 | 92.2 ms: 1.25x faster                                                        |
| pickle_dict                | 35.5 us                                                | 28.7 us: 1.24x faster                                                        |
| crypto_pyaes               | 81.9 ms                                                | 66.1 ms: 1.24x faster                                                        |
| scimark_fft                | 382 ms                                                 | 311 ms: 1.23x faster                                                         |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.19 ms: 1.21x faster                                                        |
| json_loads                 | 28.5 us                                                | 24.0 us: 1.19x faster                                                        |
| pickle                     | 11.6 us                                                | 9.82 us: 1.18x faster                                                        |
| tomli_loads                | 2.33 sec                                               | 1.98 sec: 1.18x faster                                                       |
| mako                       | 11.9 ms                                                | 10.1 ms: 1.17x faster                                                        |
| fannkuch                   | 417 ms                                                 | 358 ms: 1.16x faster                                                         |
| unpickle                   | 15.9 us                                                | 13.7 us: 1.16x faster                                                        |
| unpickle_list              | 5.29 us                                                | 4.56 us: 1.16x faster                                                        |
| async_generators           | 463 ms                                                 | 406 ms: 1.14x faster                                                         |
| meteor_contest             | 112 ms                                                 | 98.7 ms: 1.14x faster                                                        |
| json                       | 5.26 ms                                                | 4.67 ms: 1.13x faster                                                        |
| regex_dna                  | 212 ms                                                 | 188 ms: 1.13x faster                                                         |
| sympy_sum                  | 169 ms                                                 | 151 ms: 1.12x faster                                                         |
| deepcopy_memo              | 40.7 us                                                | 36.6 us: 1.11x faster                                                        |
| regex_compile              | 148 ms                                                 | 134 ms: 1.11x faster                                                         |
| gc_traversal               | 3.79 ms                                                | 3.44 ms: 1.10x faster                                                        |
| logging_format             | 7.23 us                                                | 6.63 us: 1.09x faster                                                        |
| sympy_str                  | 300 ms                                                 | 276 ms: 1.09x faster                                                         |
| json_dumps                 | 10.4 ms                                                | 9.57 ms: 1.09x faster                                                        |
| logging_simple             | 6.46 us                                                | 6.00 us: 1.08x faster                                                        |
| xml_etree_parse            | 159 ms                                                 | 148 ms: 1.08x faster                                                         |
| deepcopy                   | 371 us                                                 | 347 us: 1.07x faster                                                         |
| raytrace                   | 312 ms                                                 | 293 ms: 1.07x faster                                                         |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 682 ms: 1.06x faster                                                         |
| chaos                      | 67.0 ms                                                | 63.0 ms: 1.06x faster                                                        |
| float                      | 84.7 ms                                                | 79.8 ms: 1.06x faster                                                        |
| deepcopy_reduce            | 3.35 us                                                | 3.16 us: 1.06x faster                                                        |
| xml_etree_iterparse        | 107 ms                                                 | 101 ms: 1.06x faster                                                         |
| sqlite_synth               | 2.83 us                                                | 2.68 us: 1.06x faster                                                        |
| regex_effbot               | 3.61 ms                                                | 3.42 ms: 1.06x faster                                                        |
| pickle_pure_python         | 324 us                                                 | 308 us: 1.05x faster                                                         |
| scimark_monte_carlo        | 75.1 ms                                                | 71.6 ms: 1.05x faster                                                        |
| xml_etree_generate         | 89.2 ms                                                | 85.2 ms: 1.05x faster                                                        |
| logging_silent             | 104 ns                                                 | 100.0 ns: 1.04x faster                                                       |
| sqlglot_parse              | 1.36 ms                                                | 1.31 ms: 1.04x faster                                                        |
| xml_etree_process          | 61.7 ms                                                | 59.3 ms: 1.04x faster                                                        |
| async_tree_io_tg           | 1.18 sec                                               | 1.14 sec: 1.03x faster                                                       |
| unpickle_pure_python       | 230 us                                                 | 223 us: 1.03x faster                                                         |
| sympy_integrate            | 21.4 ms                                                | 20.9 ms: 1.03x faster                                                        |
| pprint_safe_repr           | 776 ms                                                 | 757 ms: 1.02x faster                                                         |
| async_tree_none_tg         | 450 ms                                                 | 440 ms: 1.02x faster                                                         |
| hexiom                     | 6.41 ms                                                | 6.29 ms: 1.02x faster                                                        |
| sqlglot_transpile          | 1.68 ms                                                | 1.66 ms: 1.02x faster                                                        |
| scimark_lu                 | 118 ms                                                 | 116 ms: 1.01x faster                                                         |
| sqlglot_normalize          | 110 ms                                                 | 109 ms: 1.01x faster                                                         |
| sympy_expand               | 478 ms                                                 | 473 ms: 1.01x faster                                                         |
| pprint_pformat             | 1.57 sec                                               | 1.55 sec: 1.01x faster                                                       |
| pidigits                   | 187 ms                                                 | 187 ms: 1.00x faster                                                         |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.79 sec: 1.00x slower                                                       |
| richards                   | 45.8 ms                                                | 46.7 ms: 1.02x slower                                                        |
| deltablue                  | 3.72 ms                                                | 3.80 ms: 1.02x slower                                                        |
| async_tree_memoization_tg  | 575 ms                                                 | 590 ms: 1.03x slower                                                         |
| pyflate                    | 482 ms                                                 | 496 ms: 1.03x slower                                                         |
| mdp                        | 2.63 sec                                               | 2.70 sec: 1.03x slower                                                       |
| sqlglot_optimize           | 54.8 ms                                                | 56.7 ms: 1.03x slower                                                        |
| nqueens                    | 83.3 ms                                                | 86.2 ms: 1.03x slower                                                        |
| richards_super             | 51.5 ms                                                | 53.7 ms: 1.04x slower                                                        |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.05x slower                                                       |
| async_tree_memoization     | 578 ms                                                 | 607 ms: 1.05x slower                                                         |
| regex_v8                   | 23.1 ms                                                | 24.6 ms: 1.06x slower                                                        |
| generators                 | 31.2 ms                                                | 33.6 ms: 1.08x slower                                                        |
| coroutines                 | 23.2 ms                                                | 25.0 ms: 1.08x slower                                                        |
| telco                      | 7.10 ms                                                | 7.68 ms: 1.08x slower                                                        |
| nbody                      | 97.0 ms                                                | 107 ms: 1.10x slower                                                         |
| 2to3                       | 274 ms                                                 | 304 ms: 1.11x slower                                                         |
| pycparser                  | 1.18 sec                                               | 1.32 sec: 1.12x slower                                                       |
| coverage                   | 72.7 ms                                                | 81.6 ms: 1.12x slower                                                        |
| go                         | 139 ms                                                 | 158 ms: 1.13x slower                                                         |
| mypy2                      | 830 ms                                                 | 940 ms: 1.13x slower                                                         |
| dulwich_log                | 68.5 ms                                                | 77.8 ms: 1.14x slower                                                        |
| scimark_sor                | 129 ms                                                 | 148 ms: 1.15x slower                                                         |
| asyncio_tcp                | 491 ms                                                 | 591 ms: 1.20x slower                                                         |
| pathlib                    | 19.3 ms                                                | 24.1 ms: 1.25x slower                                                        |
| asyncio_websockets         | 551 ms                                                 | 720 ms: 1.31x slower                                                         |
| dask                       | 372 ms                                                 | 495 ms: 1.33x slower                                                         |
| tornado_http               | 103 ms                                                 | 145 ms: 1.41x slower                                                         |
| bench_thread_pool          | 842 us                                                 | 1.52 ms: 1.81x slower                                                        |
| unpack_sequence            | 54.0 ns                                                | 107 ns: 1.99x slower                                                         |
| python_startup             | 9.55 ms                                                | 19.3 ms: 2.02x slower                                                        |
| python_startup_no_site     | 6.94 ms                                                | 17.8 ms: 2.56x slower                                                        |
| Geometric mean             | (ref)                                                  | 1.00x faster                                                                 |

Benchmark hidden because not significant (5): chameleon, django_template, docutils, async_tree_cpu_io_mixed, async_tree_none
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240316-3.13.0a5+-54ce2b4-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 83.23% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.15x