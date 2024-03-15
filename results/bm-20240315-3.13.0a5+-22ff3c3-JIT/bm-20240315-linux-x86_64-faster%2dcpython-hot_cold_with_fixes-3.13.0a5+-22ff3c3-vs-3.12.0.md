# Results vs. 3.12.0

- fork: faster-cpython
- ref: hot_cold_with_fixes
- machine: linux-x86_64
- commit hash: 22ff3c3
- commit date: 2024-03-15
- overall geometric mean: 1.01x slower
- HPT reliability: 86.98%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 281 ms: 1.02x slower                                                            |
| chameleon      | 7.41 ms                                                | 7.17 ms: 1.03x faster                                                           |
| tornado_http   | 103 ms                                                 | 99.3 ms: 1.03x faster                                                           |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                    |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 446 ms: 1.06x faster                                                            |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 738 ms: 1.02x slower                                                            |
| async_tree_none_tg         | 450 ms                                                 | 458 ms: 1.02x slower                                                            |
| async_tree_memoization_tg  | 575 ms                                                 | 592 ms: 1.03x slower                                                            |
| async_tree_io_tg           | 1.18 sec                                               | 1.24 sec: 1.05x slower                                                          |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.05x slower                                                          |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                                    |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 80.7 ms: 1.05x faster                                                           |
| nbody          | 97.0 ms                                                | 92.7 ms: 1.05x faster                                                           |
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                  | 1.03x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 145 ms: 1.02x faster                                                            |
| regex_effbot   | 3.61 ms                                                | 3.69 ms: 1.02x slower                                                           |
| regex_dna      | 212 ms                                                 | 228 ms: 1.07x slower                                                            |
| regex_v8       | 23.1 ms                                                | 24.9 ms: 1.08x slower                                                           |
| Geometric mean | (ref)                                                  | 1.04x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.07 sec: 1.13x faster                                                          |
| unpickle_list        | 5.29 us                                                | 4.99 us: 1.06x faster                                                           |
| pickle_pure_python   | 324 us                                                 | 312 us: 1.04x faster                                                            |
| unpickle             | 15.9 us                                                | 15.4 us: 1.03x faster                                                           |
| pickle_dict          | 35.5 us                                                | 34.7 us: 1.02x faster                                                           |
| xml_etree_process    | 61.7 ms                                                | 61.1 ms: 1.01x faster                                                           |
| xml_etree_generate   | 89.2 ms                                                | 88.6 ms: 1.01x faster                                                           |
| json_dumps           | 10.4 ms                                                | 10.4 ms: 1.00x slower                                                           |
| xml_etree_iterparse  | 107 ms                                                 | 108 ms: 1.01x slower                                                            |
| json_loads           | 28.5 us                                                | 28.9 us: 1.01x slower                                                           |
| pickle_list          | 5.08 us                                                | 5.26 us: 1.04x slower                                                           |
| unpickle_pure_python | 230 us                                                 | 238 us: 1.04x slower                                                            |
| pickle               | 11.6 us                                                | 12.1 us: 1.04x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                                    |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 11.3 ms: 1.19x slower                                                           |
| python_startup_no_site | 6.94 ms                                                | 9.93 ms: 1.43x slower                                                           |
| Geometric mean         | (ref)                                                  | 1.30x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako           | 11.9 ms                                                | 11.2 ms: 1.06x faster                                                           |
| Geometric mean | (ref)                                                  | 1.03x faster                                                                    |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 113 us: 1.40x faster                                                            |
| comprehensions             | 21.8 us                                                | 17.9 us: 1.22x faster                                                           |
| tomli_loads                | 2.33 sec                                               | 2.07 sec: 1.13x faster                                                          |
| scimark_fft                | 382 ms                                                 | 342 ms: 1.12x faster                                                            |
| crypto_pyaes               | 81.9 ms                                                | 74.6 ms: 1.10x faster                                                           |
| logging_format             | 7.23 us                                                | 6.60 us: 1.10x faster                                                           |
| logging_simple             | 6.46 us                                                | 5.95 us: 1.09x faster                                                           |
| raytrace                   | 312 ms                                                 | 290 ms: 1.08x faster                                                            |
| scimark_monte_carlo        | 75.1 ms                                                | 69.8 ms: 1.08x faster                                                           |
| deepcopy_reduce            | 3.35 us                                                | 3.13 us: 1.07x faster                                                           |
| gc_traversal               | 3.79 ms                                                | 3.57 ms: 1.06x faster                                                           |
| mako                       | 11.9 ms                                                | 11.2 ms: 1.06x faster                                                           |
| unpickle_list              | 5.29 us                                                | 4.99 us: 1.06x faster                                                           |
| async_tree_none            | 472 ms                                                 | 446 ms: 1.06x faster                                                            |
| deltablue                  | 3.72 ms                                                | 3.52 ms: 1.06x faster                                                           |
| chaos                      | 67.0 ms                                                | 63.6 ms: 1.05x faster                                                           |
| float                      | 84.7 ms                                                | 80.7 ms: 1.05x faster                                                           |
| sympy_sum                  | 169 ms                                                 | 161 ms: 1.05x faster                                                            |
| nbody                      | 97.0 ms                                                | 92.7 ms: 1.05x faster                                                           |
| deepcopy_memo              | 40.7 us                                                | 39.1 us: 1.04x faster                                                           |
| deepcopy                   | 371 us                                                 | 358 us: 1.04x faster                                                            |
| sympy_str                  | 300 ms                                                 | 289 ms: 1.04x faster                                                            |
| pickle_pure_python         | 324 us                                                 | 312 us: 1.04x faster                                                            |
| logging_silent             | 104 ns                                                 | 101 ns: 1.04x faster                                                            |
| fannkuch                   | 417 ms                                                 | 403 ms: 1.03x faster                                                            |
| chameleon                  | 7.41 ms                                                | 7.17 ms: 1.03x faster                                                           |
| tornado_http               | 103 ms                                                 | 99.3 ms: 1.03x faster                                                           |
| coroutines                 | 23.2 ms                                                | 22.5 ms: 1.03x faster                                                           |
| generators                 | 31.2 ms                                                | 30.3 ms: 1.03x faster                                                           |
| unpickle                   | 15.9 us                                                | 15.4 us: 1.03x faster                                                           |
| sqlglot_parse              | 1.36 ms                                                | 1.33 ms: 1.03x faster                                                           |
| pathlib                    | 19.3 ms                                                | 18.8 ms: 1.03x faster                                                           |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.93 ms: 1.03x faster                                                           |
| pickle_dict                | 35.5 us                                                | 34.7 us: 1.02x faster                                                           |
| pprint_safe_repr           | 776 ms                                                 | 759 ms: 1.02x faster                                                            |
| regex_compile              | 148 ms                                                 | 145 ms: 1.02x faster                                                            |
| spectral_norm              | 115 ms                                                 | 113 ms: 1.02x faster                                                            |
| xml_etree_process          | 61.7 ms                                                | 61.1 ms: 1.01x faster                                                           |
| meteor_contest             | 112 ms                                                 | 111 ms: 1.01x faster                                                            |
| pyflate                    | 482 ms                                                 | 479 ms: 1.01x faster                                                            |
| sqlglot_normalize          | 110 ms                                                 | 110 ms: 1.01x faster                                                            |
| xml_etree_generate         | 89.2 ms                                                | 88.6 ms: 1.01x faster                                                           |
| mdp                        | 2.63 sec                                               | 2.64 sec: 1.00x slower                                                          |
| json_dumps                 | 10.4 ms                                                | 10.4 ms: 1.00x slower                                                           |
| sqlite_synth               | 2.83 us                                                | 2.86 us: 1.01x slower                                                           |
| pidigits                   | 187 ms                                                 | 189 ms: 1.01x slower                                                            |
| dask                       | 372 ms                                                 | 376 ms: 1.01x slower                                                            |
| xml_etree_iterparse        | 107 ms                                                 | 108 ms: 1.01x slower                                                            |
| json_loads                 | 28.5 us                                                | 28.9 us: 1.01x slower                                                           |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 738 ms: 1.02x slower                                                            |
| async_tree_none_tg         | 450 ms                                                 | 458 ms: 1.02x slower                                                            |
| sympy_expand               | 478 ms                                                 | 489 ms: 1.02x slower                                                            |
| asyncio_websockets         | 551 ms                                                 | 564 ms: 1.02x slower                                                            |
| regex_effbot               | 3.61 ms                                                | 3.69 ms: 1.02x slower                                                           |
| richards                   | 45.8 ms                                                | 46.9 ms: 1.02x slower                                                           |
| 2to3                       | 274 ms                                                 | 281 ms: 1.02x slower                                                            |
| async_generators           | 463 ms                                                 | 475 ms: 1.03x slower                                                            |
| dulwich_log                | 68.5 ms                                                | 70.5 ms: 1.03x slower                                                           |
| async_tree_memoization_tg  | 575 ms                                                 | 592 ms: 1.03x slower                                                            |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.84 sec: 1.03x slower                                                          |
| asyncio_tcp                | 491 ms                                                 | 506 ms: 1.03x slower                                                            |
| bench_thread_pool          | 842 us                                                 | 869 us: 1.03x slower                                                            |
| bench_mp_pool              | 24.0 ms                                                | 24.8 ms: 1.03x slower                                                           |
| create_gc_cycles           | 1.48 ms                                                | 1.53 ms: 1.03x slower                                                           |
| pycparser                  | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                          |
| pickle_list                | 5.08 us                                                | 5.26 us: 1.04x slower                                                           |
| unpickle_pure_python       | 230 us                                                 | 238 us: 1.04x slower                                                            |
| pickle                     | 11.6 us                                                | 12.1 us: 1.04x slower                                                           |
| sqlglot_optimize           | 54.8 ms                                                | 57.2 ms: 1.04x slower                                                           |
| aiohttp                    | 1.15 ms                                                | 1.20 ms: 1.05x slower                                                           |
| gunicorn                   | 1.24 ms                                                | 1.30 ms: 1.05x slower                                                           |
| scimark_sor                | 129 ms                                                 | 135 ms: 1.05x slower                                                            |
| async_tree_io_tg           | 1.18 sec                                               | 1.24 sec: 1.05x slower                                                          |
| richards_super             | 51.5 ms                                                | 54.0 ms: 1.05x slower                                                           |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.05x slower                                                          |
| regex_dna                  | 212 ms                                                 | 228 ms: 1.07x slower                                                            |
| regex_v8                   | 23.1 ms                                                | 24.9 ms: 1.08x slower                                                           |
| nqueens                    | 83.3 ms                                                | 91.1 ms: 1.09x slower                                                           |
| mypy2                      | 830 ms                                                 | 911 ms: 1.10x slower                                                            |
| hexiom                     | 6.41 ms                                                | 7.17 ms: 1.12x slower                                                           |
| scimark_lu                 | 118 ms                                                 | 133 ms: 1.13x slower                                                            |
| go                         | 139 ms                                                 | 160 ms: 1.15x slower                                                            |
| python_startup             | 9.55 ms                                                | 11.3 ms: 1.19x slower                                                           |
| telco                      | 7.10 ms                                                | 8.47 ms: 1.19x slower                                                           |
| coverage                   | 72.7 ms                                                | 96.9 ms: 1.33x slower                                                           |
| python_startup_no_site     | 6.94 ms                                                | 9.93 ms: 1.43x slower                                                           |
| unpack_sequence            | 54.0 ns                                                | 85.2 ns: 1.58x slower                                                           |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                                    |

Benchmark hidden because not significant (9): sqlglot_transpile, async_tree_cpu_io_mixed, pprint_pformat, sympy_integrate, json, docutils, django_template, async_tree_memoization, xml_etree_parse
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240315-3.13.0a5+-22ff3c3-JIT/bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 86.98% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.07x