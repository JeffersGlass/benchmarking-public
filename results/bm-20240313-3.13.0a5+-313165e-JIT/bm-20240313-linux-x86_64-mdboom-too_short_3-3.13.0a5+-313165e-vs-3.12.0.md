# Results vs. 3.12.0

- fork: mdboom
- ref: too_short_3
- machine: linux-x86_64
- commit hash: 313165e
- commit date: 2024-03-13
- overall geometric mean: 1.01x slower
- HPT reliability: 82.99%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 282 ms: 1.03x slower                                          |
| chameleon      | 7.41 ms                                                | 6.86 ms: 1.08x faster                                         |
| docutils       | 2.77 sec                                               | 2.79 sec: 1.01x slower                                        |
| tornado_http   | 103 ms                                                 | 101 ms: 1.01x faster                                          |
| Geometric mean | (ref)                                                  | 1.01x faster                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 451 ms: 1.05x faster                                          |
| async_tree_none_tg         | 450 ms                                                 | 456 ms: 1.01x slower                                          |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 738 ms: 1.02x slower                                          |
| async_tree_memoization_tg  | 575 ms                                                 | 587 ms: 1.02x slower                                          |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                        |
| async_tree_io              | 1.16 sec                                               | 1.20 sec: 1.04x slower                                        |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                  |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| float          | 84.7 ms                                                | 79.9 ms: 1.06x faster                                         |
| nbody          | 97.0 ms                                                | 94.0 ms: 1.03x faster                                         |
| pidigits       | 187 ms                                                 | 190 ms: 1.02x slower                                          |
| Geometric mean | (ref)                                                  | 1.03x faster                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 142 ms: 1.04x faster                                          |
| regex_effbot   | 3.61 ms                                                | 3.59 ms: 1.01x faster                                         |
| regex_dna      | 212 ms                                                 | 220 ms: 1.04x slower                                          |
| regex_v8       | 23.1 ms                                                | 24.1 ms: 1.04x slower                                         |
| Geometric mean | (ref)                                                  | 1.01x slower                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.12 sec: 1.10x faster                                        |
| unpickle_list        | 5.29 us                                                | 4.91 us: 1.08x faster                                         |
| unpickle             | 15.9 us                                                | 14.7 us: 1.08x faster                                         |
| pickle_pure_python   | 324 us                                                 | 302 us: 1.07x faster                                          |
| pickle_dict          | 35.5 us                                                | 33.9 us: 1.05x faster                                         |
| xml_etree_process    | 61.7 ms                                                | 59.8 ms: 1.03x faster                                         |
| json_loads           | 28.5 us                                                | 28.0 us: 1.02x faster                                         |
| pickle_list          | 5.08 us                                                | 4.99 us: 1.02x faster                                         |
| xml_etree_generate   | 89.2 ms                                                | 87.8 ms: 1.02x faster                                         |
| pickle               | 11.6 us                                                | 11.6 us: 1.00x faster                                         |
| xml_etree_parse      | 159 ms                                                 | 161 ms: 1.01x slower                                          |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                         |
| xml_etree_iterparse  | 107 ms                                                 | 108 ms: 1.02x slower                                          |
| unpickle_pure_python | 230 us                                                 | 243 us: 1.06x slower                                          |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.6 ms: 1.32x slower                                         |
| python_startup_no_site | 6.94 ms                                                | 11.1 ms: 1.61x slower                                         |
| Geometric mean         | (ref)                                                  | 1.46x slower                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| mako           | 11.9 ms                                                | 10.7 ms: 1.11x faster                                         |
| Geometric mean | (ref)                                                  | 1.05x faster                                                  |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 112 us: 1.41x faster                                          |
| comprehensions             | 21.8 us                                                | 17.4 us: 1.25x faster                                         |
| logging_format             | 7.23 us                                                | 6.40 us: 1.13x faster                                         |
| scimark_fft                | 382 ms                                                 | 342 ms: 1.12x faster                                          |
| mako                       | 11.9 ms                                                | 10.7 ms: 1.11x faster                                         |
| logging_simple             | 6.46 us                                                | 5.86 us: 1.10x faster                                         |
| tomli_loads                | 2.33 sec                                               | 2.12 sec: 1.10x faster                                        |
| crypto_pyaes               | 81.9 ms                                                | 75.7 ms: 1.08x faster                                         |
| chameleon                  | 7.41 ms                                                | 6.86 ms: 1.08x faster                                         |
| unpickle_list              | 5.29 us                                                | 4.91 us: 1.08x faster                                         |
| unpickle                   | 15.9 us                                                | 14.7 us: 1.08x faster                                         |
| raytrace                   | 312 ms                                                 | 290 ms: 1.08x faster                                          |
| pickle_pure_python         | 324 us                                                 | 302 us: 1.07x faster                                          |
| deepcopy_reduce            | 3.35 us                                                | 3.12 us: 1.07x faster                                         |
| deltablue                  | 3.72 ms                                                | 3.47 ms: 1.07x faster                                         |
| float                      | 84.7 ms                                                | 79.9 ms: 1.06x faster                                         |
| deepcopy                   | 371 us                                                 | 352 us: 1.05x faster                                          |
| generators                 | 31.2 ms                                                | 29.6 ms: 1.05x faster                                         |
| fannkuch                   | 417 ms                                                 | 396 ms: 1.05x faster                                          |
| pickle_dict                | 35.5 us                                                | 33.9 us: 1.05x faster                                         |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.83 ms: 1.05x faster                                         |
| scimark_monte_carlo        | 75.1 ms                                                | 71.8 ms: 1.05x faster                                         |
| async_tree_none            | 472 ms                                                 | 451 ms: 1.05x faster                                          |
| regex_compile              | 148 ms                                                 | 142 ms: 1.04x faster                                          |
| deepcopy_memo              | 40.7 us                                                | 39.1 us: 1.04x faster                                         |
| sympy_sum                  | 169 ms                                                 | 163 ms: 1.04x faster                                          |
| sympy_str                  | 300 ms                                                 | 288 ms: 1.04x faster                                          |
| sqlglot_parse              | 1.36 ms                                                | 1.32 ms: 1.03x faster                                         |
| xml_etree_process          | 61.7 ms                                                | 59.8 ms: 1.03x faster                                         |
| nbody                      | 97.0 ms                                                | 94.0 ms: 1.03x faster                                         |
| pathlib                    | 19.3 ms                                                | 18.8 ms: 1.03x faster                                         |
| chaos                      | 67.0 ms                                                | 65.1 ms: 1.03x faster                                         |
| gc_traversal               | 3.79 ms                                                | 3.69 ms: 1.03x faster                                         |
| coroutines                 | 23.2 ms                                                | 22.7 ms: 1.02x faster                                         |
| json_loads                 | 28.5 us                                                | 28.0 us: 1.02x faster                                         |
| pickle_list                | 5.08 us                                                | 4.99 us: 1.02x faster                                         |
| meteor_contest             | 112 ms                                                 | 111 ms: 1.02x faster                                          |
| sqlglot_transpile          | 1.68 ms                                                | 1.66 ms: 1.02x faster                                         |
| xml_etree_generate         | 89.2 ms                                                | 87.8 ms: 1.02x faster                                         |
| logging_silent             | 104 ns                                                 | 103 ns: 1.01x faster                                          |
| tornado_http               | 103 ms                                                 | 101 ms: 1.01x faster                                          |
| spectral_norm              | 115 ms                                                 | 114 ms: 1.01x faster                                          |
| regex_effbot               | 3.61 ms                                                | 3.59 ms: 1.01x faster                                         |
| mdp                        | 2.63 sec                                               | 2.62 sec: 1.00x faster                                        |
| pickle                     | 11.6 us                                                | 11.6 us: 1.00x faster                                         |
| pyflate                    | 482 ms                                                 | 486 ms: 1.01x slower                                          |
| docutils                   | 2.77 sec                                               | 2.79 sec: 1.01x slower                                        |
| xml_etree_parse            | 159 ms                                                 | 161 ms: 1.01x slower                                          |
| sympy_integrate            | 21.4 ms                                                | 21.6 ms: 1.01x slower                                         |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                         |
| async_tree_none_tg         | 450 ms                                                 | 456 ms: 1.01x slower                                          |
| pidigits                   | 187 ms                                                 | 190 ms: 1.02x slower                                          |
| xml_etree_iterparse        | 107 ms                                                 | 108 ms: 1.02x slower                                          |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 738 ms: 1.02x slower                                          |
| asyncio_websockets         | 551 ms                                                 | 562 ms: 1.02x slower                                          |
| sympy_expand               | 478 ms                                                 | 487 ms: 1.02x slower                                          |
| async_generators           | 463 ms                                                 | 472 ms: 1.02x slower                                          |
| async_tree_memoization_tg  | 575 ms                                                 | 587 ms: 1.02x slower                                          |
| create_gc_cycles           | 1.48 ms                                                | 1.51 ms: 1.02x slower                                         |
| dulwich_log                | 68.5 ms                                                | 70.2 ms: 1.02x slower                                         |
| asyncio_tcp                | 491 ms                                                 | 503 ms: 1.03x slower                                          |
| 2to3                       | 274 ms                                                 | 282 ms: 1.03x slower                                          |
| bench_thread_pool          | 842 us                                                 | 866 us: 1.03x slower                                          |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.85 sec: 1.03x slower                                        |
| richards_super             | 51.5 ms                                                | 53.3 ms: 1.03x slower                                         |
| pycparser                  | 1.18 sec                                               | 1.22 sec: 1.03x slower                                        |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                        |
| regex_dna                  | 212 ms                                                 | 220 ms: 1.04x slower                                          |
| async_tree_io              | 1.16 sec                                               | 1.20 sec: 1.04x slower                                        |
| sqlglot_optimize           | 54.8 ms                                                | 56.9 ms: 1.04x slower                                         |
| regex_v8                   | 23.1 ms                                                | 24.1 ms: 1.04x slower                                         |
| richards                   | 45.8 ms                                                | 48.0 ms: 1.05x slower                                         |
| gunicorn                   | 1.24 ms                                                | 1.30 ms: 1.05x slower                                         |
| aiohttp                    | 1.15 ms                                                | 1.21 ms: 1.05x slower                                         |
| unpickle_pure_python       | 230 us                                                 | 243 us: 1.06x slower                                          |
| nqueens                    | 83.3 ms                                                | 89.7 ms: 1.08x slower                                         |
| bench_mp_pool              | 24.0 ms                                                | 26.3 ms: 1.10x slower                                         |
| hexiom                     | 6.41 ms                                                | 7.06 ms: 1.10x slower                                         |
| scimark_lu                 | 118 ms                                                 | 131 ms: 1.11x slower                                          |
| go                         | 139 ms                                                 | 157 ms: 1.13x slower                                          |
| telco                      | 7.10 ms                                                | 8.41 ms: 1.18x slower                                         |
| python_startup             | 9.55 ms                                                | 12.6 ms: 1.32x slower                                         |
| coverage                   | 72.7 ms                                                | 97.4 ms: 1.34x slower                                         |
| python_startup_no_site     | 6.94 ms                                                | 11.1 ms: 1.61x slower                                         |
| unpack_sequence            | 54.0 ns                                                | 87.5 ns: 1.62x slower                                         |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                  |

Benchmark hidden because not significant (11): json, async_tree_memoization, pprint_pformat, django_template, pprint_safe_repr, sqlglot_normalize, scimark_sor, sqlite_synth, dask, async_tree_cpu_io_mixed, mypy2
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240313-3.13.0a5+-313165e-JIT/bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 82.99% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.17x