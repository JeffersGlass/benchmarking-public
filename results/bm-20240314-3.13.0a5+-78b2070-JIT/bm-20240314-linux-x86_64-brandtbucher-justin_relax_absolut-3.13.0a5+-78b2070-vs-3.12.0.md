# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_relax_absolut
- machine: linux-x86_64
- commit hash: 78b2070
- commit date: 2024-03-14
- overall geometric mean: 1.01x slower
- HPT reliability: 95.43%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 284 ms: 1.03x slower                                                         |
| chameleon      | 7.41 ms                                                | 6.96 ms: 1.07x faster                                                        |
| tornado_http   | 103 ms                                                 | 99.1 ms: 1.04x faster                                                        |
| Geometric mean | (ref)                                                  | 1.02x faster                                                                 |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 448 ms: 1.05x faster                                                         |
| async_tree_none_tg         | 450 ms                                                 | 459 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 744 ms: 1.03x slower                                                         |
| async_tree_memoization_tg  | 575 ms                                                 | 595 ms: 1.04x slower                                                         |
| async_tree_io_tg           | 1.18 sec                                               | 1.23 sec: 1.04x slower                                                       |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.05x slower                                                       |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                                 |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 92.6 ms: 1.05x faster                                                        |
| float          | 84.7 ms                                                | 81.3 ms: 1.04x faster                                                        |
| pidigits       | 187 ms                                                 | 190 ms: 1.02x slower                                                         |
| Geometric mean | (ref)                                                  | 1.02x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 144 ms: 1.03x faster                                                         |
| regex_effbot   | 3.61 ms                                                | 3.65 ms: 1.01x slower                                                        |
| regex_v8       | 23.1 ms                                                | 24.0 ms: 1.04x slower                                                        |
| regex_dna      | 212 ms                                                 | 225 ms: 1.06x slower                                                         |
| Geometric mean | (ref)                                                  | 1.02x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.05 sec: 1.14x faster                                                       |
| unpickle_list        | 5.29 us                                                | 4.81 us: 1.10x faster                                                        |
| pickle_pure_python   | 324 us                                                 | 301 us: 1.08x faster                                                         |
| pickle_list          | 5.08 us                                                | 4.81 us: 1.06x faster                                                        |
| pickle_dict          | 35.5 us                                                | 34.9 us: 1.02x faster                                                        |
| xml_etree_process    | 61.7 ms                                                | 60.6 ms: 1.02x faster                                                        |
| xml_etree_generate   | 89.2 ms                                                | 88.1 ms: 1.01x faster                                                        |
| xml_etree_parse      | 159 ms                                                 | 161 ms: 1.01x slower                                                         |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                        |
| pickle               | 11.6 us                                                | 11.8 us: 1.02x slower                                                        |
| xml_etree_iterparse  | 107 ms                                                 | 109 ms: 1.02x slower                                                         |
| unpickle_pure_python | 230 us                                                 | 245 us: 1.07x slower                                                         |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                                 |

Benchmark hidden because not significant (2): unpickle, json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.6 ms: 1.32x slower                                                        |
| python_startup_no_site | 6.94 ms                                                | 11.2 ms: 1.61x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.46x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 10.9 ms: 1.09x faster                                                        |
| django_template | 34.6 ms                                                | 34.2 ms: 1.01x faster                                                        |
| Geometric mean  | (ref)                                                  | 1.05x faster                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 112 us: 1.41x faster                                                         |
| comprehensions             | 21.8 us                                                | 17.9 us: 1.22x faster                                                        |
| tomli_loads                | 2.33 sec                                               | 2.05 sec: 1.14x faster                                                       |
| logging_format             | 7.23 us                                                | 6.40 us: 1.13x faster                                                        |
| logging_simple             | 6.46 us                                                | 5.83 us: 1.11x faster                                                        |
| scimark_fft                | 382 ms                                                 | 346 ms: 1.11x faster                                                         |
| unpickle_list              | 5.29 us                                                | 4.81 us: 1.10x faster                                                        |
| deepcopy_reduce            | 3.35 us                                                | 3.04 us: 1.10x faster                                                        |
| mako                       | 11.9 ms                                                | 10.9 ms: 1.09x faster                                                        |
| pickle_pure_python         | 324 us                                                 | 301 us: 1.08x faster                                                         |
| deltablue                  | 3.72 ms                                                | 3.48 ms: 1.07x faster                                                        |
| chameleon                  | 7.41 ms                                                | 6.96 ms: 1.07x faster                                                        |
| crypto_pyaes               | 81.9 ms                                                | 77.3 ms: 1.06x faster                                                        |
| pickle_list                | 5.08 us                                                | 4.81 us: 1.06x faster                                                        |
| async_tree_none            | 472 ms                                                 | 448 ms: 1.05x faster                                                         |
| generators                 | 31.2 ms                                                | 29.7 ms: 1.05x faster                                                        |
| nbody                      | 97.0 ms                                                | 92.6 ms: 1.05x faster                                                        |
| deepcopy                   | 371 us                                                 | 355 us: 1.05x faster                                                         |
| pathlib                    | 19.3 ms                                                | 18.5 ms: 1.05x faster                                                        |
| sympy_str                  | 300 ms                                                 | 287 ms: 1.04x faster                                                         |
| logging_silent             | 104 ns                                                 | 100 ns: 1.04x faster                                                         |
| sympy_sum                  | 169 ms                                                 | 162 ms: 1.04x faster                                                         |
| float                      | 84.7 ms                                                | 81.3 ms: 1.04x faster                                                        |
| sqlglot_parse              | 1.36 ms                                                | 1.31 ms: 1.04x faster                                                        |
| tornado_http               | 103 ms                                                 | 99.1 ms: 1.04x faster                                                        |
| fannkuch                   | 417 ms                                                 | 403 ms: 1.04x faster                                                         |
| raytrace                   | 312 ms                                                 | 302 ms: 1.03x faster                                                         |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.89 ms: 1.03x faster                                                        |
| deepcopy_memo              | 40.7 us                                                | 39.4 us: 1.03x faster                                                        |
| pprint_safe_repr           | 776 ms                                                 | 751 ms: 1.03x faster                                                         |
| regex_compile              | 148 ms                                                 | 144 ms: 1.03x faster                                                         |
| scimark_monte_carlo        | 75.1 ms                                                | 73.1 ms: 1.03x faster                                                        |
| chaos                      | 67.0 ms                                                | 65.3 ms: 1.03x faster                                                        |
| pickle_dict                | 35.5 us                                                | 34.9 us: 1.02x faster                                                        |
| xml_etree_process          | 61.7 ms                                                | 60.6 ms: 1.02x faster                                                        |
| sqlglot_transpile          | 1.68 ms                                                | 1.65 ms: 1.02x faster                                                        |
| coroutines                 | 23.2 ms                                                | 22.8 ms: 1.02x faster                                                        |
| sqlglot_normalize          | 110 ms                                                 | 109 ms: 1.01x faster                                                         |
| django_template            | 34.6 ms                                                | 34.2 ms: 1.01x faster                                                        |
| xml_etree_generate         | 89.2 ms                                                | 88.1 ms: 1.01x faster                                                        |
| meteor_contest             | 112 ms                                                 | 111 ms: 1.01x faster                                                         |
| sympy_integrate            | 21.4 ms                                                | 21.2 ms: 1.01x faster                                                        |
| gc_traversal               | 3.79 ms                                                | 3.81 ms: 1.01x slower                                                        |
| xml_etree_parse            | 159 ms                                                 | 161 ms: 1.01x slower                                                         |
| mdp                        | 2.63 sec                                               | 2.65 sec: 1.01x slower                                                       |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                        |
| asyncio_tcp                | 491 ms                                                 | 495 ms: 1.01x slower                                                         |
| regex_effbot               | 3.61 ms                                                | 3.65 ms: 1.01x slower                                                        |
| scimark_sor                | 129 ms                                                 | 131 ms: 1.01x slower                                                         |
| pidigits                   | 187 ms                                                 | 190 ms: 1.02x slower                                                         |
| pickle                     | 11.6 us                                                | 11.8 us: 1.02x slower                                                        |
| async_generators           | 463 ms                                                 | 471 ms: 1.02x slower                                                         |
| sympy_expand               | 478 ms                                                 | 487 ms: 1.02x slower                                                         |
| asyncio_websockets         | 551 ms                                                 | 562 ms: 1.02x slower                                                         |
| xml_etree_iterparse        | 107 ms                                                 | 109 ms: 1.02x slower                                                         |
| dulwich_log                | 68.5 ms                                                | 69.9 ms: 1.02x slower                                                        |
| async_tree_none_tg         | 450 ms                                                 | 459 ms: 1.02x slower                                                         |
| bench_thread_pool          | 842 us                                                 | 860 us: 1.02x slower                                                         |
| spectral_norm              | 115 ms                                                 | 118 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 744 ms: 1.03x slower                                                         |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.85 sec: 1.03x slower                                                       |
| 2to3                       | 274 ms                                                 | 284 ms: 1.03x slower                                                         |
| async_tree_memoization_tg  | 575 ms                                                 | 595 ms: 1.04x slower                                                         |
| sqlglot_optimize           | 54.8 ms                                                | 56.8 ms: 1.04x slower                                                        |
| pycparser                  | 1.18 sec                                               | 1.22 sec: 1.04x slower                                                       |
| regex_v8                   | 23.1 ms                                                | 24.0 ms: 1.04x slower                                                        |
| richards_super             | 51.5 ms                                                | 53.5 ms: 1.04x slower                                                        |
| async_tree_io_tg           | 1.18 sec                                               | 1.23 sec: 1.04x slower                                                       |
| richards                   | 45.8 ms                                                | 47.7 ms: 1.04x slower                                                        |
| pyflate                    | 482 ms                                                 | 503 ms: 1.04x slower                                                         |
| gunicorn                   | 1.24 ms                                                | 1.30 ms: 1.04x slower                                                        |
| aiohttp                    | 1.15 ms                                                | 1.20 ms: 1.05x slower                                                        |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.05x slower                                                       |
| create_gc_cycles           | 1.48 ms                                                | 1.55 ms: 1.05x slower                                                        |
| regex_dna                  | 212 ms                                                 | 225 ms: 1.06x slower                                                         |
| unpickle_pure_python       | 230 us                                                 | 245 us: 1.07x slower                                                         |
| nqueens                    | 83.3 ms                                                | 90.8 ms: 1.09x slower                                                        |
| bench_mp_pool              | 24.0 ms                                                | 26.4 ms: 1.10x slower                                                        |
| scimark_lu                 | 118 ms                                                 | 134 ms: 1.13x slower                                                         |
| go                         | 139 ms                                                 | 158 ms: 1.14x slower                                                         |
| hexiom                     | 6.41 ms                                                | 7.29 ms: 1.14x slower                                                        |
| telco                      | 7.10 ms                                                | 8.48 ms: 1.19x slower                                                        |
| python_startup             | 9.55 ms                                                | 12.6 ms: 1.32x slower                                                        |
| coverage                   | 72.7 ms                                                | 97.4 ms: 1.34x slower                                                        |
| python_startup_no_site     | 6.94 ms                                                | 11.2 ms: 1.61x slower                                                        |
| unpack_sequence            | 54.0 ns                                                | 87.8 ns: 1.63x slower                                                        |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                                 |

Benchmark hidden because not significant (10): unpickle, json, json_loads, async_tree_memoization, sqlite_synth, dask, docutils, async_tree_cpu_io_mixed, pprint_pformat, mypy2
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240314-3.13.0a5+-78b2070-JIT/bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 95.43% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.17x