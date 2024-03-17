# Results vs. 3.12.0

- fork: jeffersglass
- ref: justin_supernodes_on
- machine: linux-x86_64
- commit hash: f486338
- commit date: 2024-03-16
- overall geometric mean: 1.01x faster
- HPT reliability: 98.51%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.16x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 297 ms: 1.08x slower                                                         |
| chameleon      | 7.41 ms                                                | 7.25 ms: 1.02x faster                                                        |
| docutils       | 2.77 sec                                               | 2.67 sec: 1.04x faster                                                       |
| tornado_http   | 103 ms                                                 | 147 ms: 1.43x slower                                                         |
| Geometric mean | (ref)                                                  | 1.10x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.18 sec                                               | 1.10 sec: 1.08x faster                                                       |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 677 ms: 1.07x faster                                                         |
| async_tree_none            | 472 ms                                                 | 449 ms: 1.05x faster                                                         |
| async_tree_none_tg         | 450 ms                                                 | 428 ms: 1.05x faster                                                         |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 698 ms: 1.04x faster                                                         |
| Geometric mean             | (ref)                                                  | 1.04x faster                                                                 |

Benchmark hidden because not significant (3): async_tree_memoization_tg, async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 78.5 ms: 1.08x faster                                                        |
| pidigits       | 187 ms                                                 | 188 ms: 1.01x slower                                                         |
| nbody          | 97.0 ms                                                | 103 ms: 1.06x slower                                                         |
| Geometric mean | (ref)                                                  | 1.00x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 212 ms                                                 | 191 ms: 1.11x faster                                                         |
| regex_compile  | 148 ms                                                 | 136 ms: 1.09x faster                                                         |
| regex_effbot   | 3.61 ms                                                | 3.37 ms: 1.07x faster                                                        |
| regex_v8       | 23.1 ms                                                | 23.8 ms: 1.03x slower                                                        |
| Geometric mean | (ref)                                                  | 1.06x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_list          | 5.08 us                                                | 3.76 us: 1.35x faster                                                        |
| pickle_dict          | 35.5 us                                                | 27.8 us: 1.28x faster                                                        |
| tomli_loads          | 2.33 sec                                               | 1.93 sec: 1.21x faster                                                       |
| json_loads           | 28.5 us                                                | 23.9 us: 1.19x faster                                                        |
| unpickle_list        | 5.29 us                                                | 4.43 us: 1.19x faster                                                        |
| pickle               | 11.6 us                                                | 9.75 us: 1.19x faster                                                        |
| unpickle             | 15.9 us                                                | 13.5 us: 1.17x faster                                                        |
| json_dumps           | 10.4 ms                                                | 9.56 ms: 1.09x faster                                                        |
| xml_etree_parse      | 159 ms                                                 | 147 ms: 1.08x faster                                                         |
| pickle_pure_python   | 324 us                                                 | 304 us: 1.07x faster                                                         |
| xml_etree_iterparse  | 107 ms                                                 | 100 ms: 1.06x faster                                                         |
| xml_etree_generate   | 89.2 ms                                                | 85.3 ms: 1.05x faster                                                        |
| unpickle_pure_python | 230 us                                                 | 223 us: 1.03x faster                                                         |
| xml_etree_process    | 61.7 ms                                                | 59.9 ms: 1.03x faster                                                        |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 19.2 ms: 2.01x slower                                                        |
| python_startup_no_site | 6.94 ms                                                | 17.8 ms: 2.56x slower                                                        |
| Geometric mean         | (ref)                                                  | 2.27x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako           | 11.9 ms                                                | 9.85 ms: 1.21x faster                                                        |
| Geometric mean | (ref)                                                  | 1.10x faster                                                                 |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| bench_mp_pool              | 24.0 ms                                                | 16.0 ms: 1.50x faster                                                        |
| typing_runtime_protocols   | 158 us                                                 | 111 us: 1.43x faster                                                         |
| pickle_list                | 5.08 us                                                | 3.76 us: 1.35x faster                                                        |
| create_gc_cycles           | 1.48 ms                                                | 1.10 ms: 1.34x faster                                                        |
| comprehensions             | 21.8 us                                                | 16.4 us: 1.33x faster                                                        |
| pickle_dict                | 35.5 us                                                | 27.8 us: 1.28x faster                                                        |
| scimark_fft                | 382 ms                                                 | 303 ms: 1.26x faster                                                         |
| crypto_pyaes               | 81.9 ms                                                | 65.4 ms: 1.25x faster                                                        |
| spectral_norm              | 115 ms                                                 | 92.7 ms: 1.24x faster                                                        |
| fannkuch                   | 417 ms                                                 | 343 ms: 1.21x faster                                                         |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.16 ms: 1.21x faster                                                        |
| mako                       | 11.9 ms                                                | 9.85 ms: 1.21x faster                                                        |
| tomli_loads                | 2.33 sec                                               | 1.93 sec: 1.21x faster                                                       |
| json_loads                 | 28.5 us                                                | 23.9 us: 1.19x faster                                                        |
| unpickle_list              | 5.29 us                                                | 4.43 us: 1.19x faster                                                        |
| pickle                     | 11.6 us                                                | 9.75 us: 1.19x faster                                                        |
| unpickle                   | 15.9 us                                                | 13.5 us: 1.17x faster                                                        |
| gc_traversal               | 3.79 ms                                                | 3.27 ms: 1.16x faster                                                        |
| json                       | 5.26 ms                                                | 4.58 ms: 1.15x faster                                                        |
| async_generators           | 463 ms                                                 | 405 ms: 1.14x faster                                                         |
| deepcopy_memo              | 40.7 us                                                | 36.3 us: 1.12x faster                                                        |
| meteor_contest             | 112 ms                                                 | 101 ms: 1.12x faster                                                         |
| sympy_sum                  | 169 ms                                                 | 152 ms: 1.11x faster                                                         |
| regex_dna                  | 212 ms                                                 | 191 ms: 1.11x faster                                                         |
| regex_compile              | 148 ms                                                 | 136 ms: 1.09x faster                                                         |
| chaos                      | 67.0 ms                                                | 61.3 ms: 1.09x faster                                                        |
| deepcopy                   | 371 us                                                 | 340 us: 1.09x faster                                                         |
| logging_format             | 7.23 us                                                | 6.64 us: 1.09x faster                                                        |
| raytrace                   | 312 ms                                                 | 287 ms: 1.09x faster                                                         |
| sympy_str                  | 300 ms                                                 | 276 ms: 1.09x faster                                                         |
| json_dumps                 | 10.4 ms                                                | 9.56 ms: 1.09x faster                                                        |
| xml_etree_parse            | 159 ms                                                 | 147 ms: 1.08x faster                                                         |
| scimark_monte_carlo        | 75.1 ms                                                | 69.6 ms: 1.08x faster                                                        |
| float                      | 84.7 ms                                                | 78.5 ms: 1.08x faster                                                        |
| async_tree_io_tg           | 1.18 sec                                               | 1.10 sec: 1.08x faster                                                       |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 677 ms: 1.07x faster                                                         |
| regex_effbot               | 3.61 ms                                                | 3.37 ms: 1.07x faster                                                        |
| deepcopy_reduce            | 3.35 us                                                | 3.13 us: 1.07x faster                                                        |
| pickle_pure_python         | 324 us                                                 | 304 us: 1.07x faster                                                         |
| xml_etree_iterparse        | 107 ms                                                 | 100 ms: 1.06x faster                                                         |
| logging_simple             | 6.46 us                                                | 6.09 us: 1.06x faster                                                        |
| sqlite_synth               | 2.83 us                                                | 2.69 us: 1.05x faster                                                        |
| async_tree_none            | 472 ms                                                 | 449 ms: 1.05x faster                                                         |
| async_tree_none_tg         | 450 ms                                                 | 428 ms: 1.05x faster                                                         |
| xml_etree_generate         | 89.2 ms                                                | 85.3 ms: 1.05x faster                                                        |
| sqlglot_parse              | 1.36 ms                                                | 1.30 ms: 1.04x faster                                                        |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 698 ms: 1.04x faster                                                         |
| mdp                        | 2.63 sec                                               | 2.54 sec: 1.04x faster                                                       |
| docutils                   | 2.77 sec                                               | 2.67 sec: 1.04x faster                                                       |
| pprint_safe_repr           | 776 ms                                                 | 750 ms: 1.03x faster                                                         |
| unpickle_pure_python       | 230 us                                                 | 223 us: 1.03x faster                                                         |
| xml_etree_process          | 61.7 ms                                                | 59.9 ms: 1.03x faster                                                        |
| hexiom                     | 6.41 ms                                                | 6.26 ms: 1.02x faster                                                        |
| sqlglot_transpile          | 1.68 ms                                                | 1.65 ms: 1.02x faster                                                        |
| chameleon                  | 7.41 ms                                                | 7.25 ms: 1.02x faster                                                        |
| sympy_integrate            | 21.4 ms                                                | 21.0 ms: 1.02x faster                                                        |
| sympy_expand               | 478 ms                                                 | 469 ms: 1.02x faster                                                         |
| logging_silent             | 104 ns                                                 | 103 ns: 1.02x faster                                                         |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.76 sec: 1.01x faster                                                       |
| pprint_pformat             | 1.57 sec                                               | 1.55 sec: 1.01x faster                                                       |
| sqlglot_normalize          | 110 ms                                                 | 109 ms: 1.01x faster                                                         |
| pidigits                   | 187 ms                                                 | 188 ms: 1.01x slower                                                         |
| deltablue                  | 3.72 ms                                                | 3.75 ms: 1.01x slower                                                        |
| pyflate                    | 482 ms                                                 | 489 ms: 1.01x slower                                                         |
| richards                   | 45.8 ms                                                | 46.8 ms: 1.02x slower                                                        |
| regex_v8                   | 23.1 ms                                                | 23.8 ms: 1.03x slower                                                        |
| nqueens                    | 83.3 ms                                                | 86.3 ms: 1.04x slower                                                        |
| sqlglot_optimize           | 54.8 ms                                                | 56.9 ms: 1.04x slower                                                        |
| richards_super             | 51.5 ms                                                | 54.3 ms: 1.05x slower                                                        |
| nbody                      | 97.0 ms                                                | 103 ms: 1.06x slower                                                         |
| telco                      | 7.10 ms                                                | 7.63 ms: 1.07x slower                                                        |
| 2to3                       | 274 ms                                                 | 297 ms: 1.08x slower                                                         |
| coverage                   | 72.7 ms                                                | 78.8 ms: 1.08x slower                                                        |
| coroutines                 | 23.2 ms                                                | 25.4 ms: 1.10x slower                                                        |
| pycparser                  | 1.18 sec                                               | 1.31 sec: 1.11x slower                                                       |
| mypy2                      | 830 ms                                                 | 928 ms: 1.12x slower                                                         |
| scimark_sor                | 129 ms                                                 | 146 ms: 1.13x slower                                                         |
| go                         | 139 ms                                                 | 159 ms: 1.14x slower                                                         |
| dulwich_log                | 68.5 ms                                                | 78.2 ms: 1.14x slower                                                        |
| asyncio_tcp                | 491 ms                                                 | 592 ms: 1.21x slower                                                         |
| pathlib                    | 19.3 ms                                                | 24.2 ms: 1.25x slower                                                        |
| dask                       | 372 ms                                                 | 483 ms: 1.30x slower                                                         |
| asyncio_websockets         | 551 ms                                                 | 721 ms: 1.31x slower                                                         |
| tornado_http               | 103 ms                                                 | 147 ms: 1.43x slower                                                         |
| bench_thread_pool          | 842 us                                                 | 1.51 ms: 1.79x slower                                                        |
| python_startup             | 9.55 ms                                                | 19.2 ms: 2.01x slower                                                        |
| unpack_sequence            | 54.0 ns                                                | 110 ns: 2.04x slower                                                         |
| python_startup_no_site     | 6.94 ms                                                | 17.8 ms: 2.56x slower                                                        |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                                 |

Benchmark hidden because not significant (6): async_tree_memoization_tg, django_template, scimark_lu, generators, async_tree_io, async_tree_memoization
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240316-3.13.0a5+-f486338-JIT/bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 98.51% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.16x