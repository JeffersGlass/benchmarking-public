# Results vs. 3.12.0

- fork: python
- ref: 61e54bfcee9f08a8e09a
- machine: linux-x86_64
- commit hash: 61e54bf
- commit date: 2024-03-14
- overall geometric mean: 1.01x slower
- HPT reliability: 86.98%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 282 ms: 1.03x slower                                                   |
| chameleon      | 7.41 ms                                                | 6.96 ms: 1.06x faster                                                  |
| docutils       | 2.77 sec                                               | 2.78 sec: 1.00x slower                                                 |
| tornado_http   | 103 ms                                                 | 99.0 ms: 1.04x faster                                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 447 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 743 ms: 1.02x slower                                                   |
| async_tree_none_tg         | 450 ms                                                 | 461 ms: 1.03x slower                                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 597 ms: 1.04x slower                                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.24 sec: 1.05x slower                                                 |
| async_tree_io              | 1.16 sec                                               | 1.22 sec: 1.05x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                           |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 80.0 ms: 1.06x faster                                                  |
| nbody          | 97.0 ms                                                | 92.7 ms: 1.05x faster                                                  |
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                   |
| Geometric mean | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 143 ms: 1.04x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.79 ms: 1.05x slower                                                  |
| regex_dna      | 212 ms                                                 | 234 ms: 1.10x slower                                                   |
| regex_v8       | 23.1 ms                                                | 25.9 ms: 1.12x slower                                                  |
| Geometric mean | (ref)                                                  | 1.06x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.07 sec: 1.12x faster                                                 |
| unpickle_list        | 5.29 us                                                | 4.93 us: 1.07x faster                                                  |
| pickle_pure_python   | 324 us                                                 | 308 us: 1.05x faster                                                   |
| unpickle             | 15.9 us                                                | 15.4 us: 1.03x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 60.6 ms: 1.02x faster                                                  |
| json_loads           | 28.5 us                                                | 28.1 us: 1.01x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 88.6 ms: 1.01x faster                                                  |
| pickle_dict          | 35.5 us                                                | 35.4 us: 1.00x faster                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 108 ms: 1.02x slower                                                   |
| json_dumps           | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                  |
| pickle               | 11.6 us                                                | 11.9 us: 1.03x slower                                                  |
| unpickle_pure_python | 230 us                                                 | 239 us: 1.04x slower                                                   |
| pickle_list          | 5.08 us                                                | 5.29 us: 1.04x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.6 ms: 1.32x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 11.2 ms: 1.61x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.45x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako           | 11.9 ms                                                | 11.1 ms: 1.07x faster                                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 111 us: 1.42x faster                                                   |
| comprehensions             | 21.8 us                                                | 17.5 us: 1.24x faster                                                  |
| logging_format             | 7.23 us                                                | 6.42 us: 1.13x faster                                                  |
| tomli_loads                | 2.33 sec                                               | 2.07 sec: 1.12x faster                                                 |
| logging_simple             | 6.46 us                                                | 5.77 us: 1.12x faster                                                  |
| scimark_fft                | 382 ms                                                 | 345 ms: 1.11x faster                                                   |
| deepcopy_reduce            | 3.35 us                                                | 3.06 us: 1.09x faster                                                  |
| deltablue                  | 3.72 ms                                                | 3.42 ms: 1.09x faster                                                  |
| unpickle_list              | 5.29 us                                                | 4.93 us: 1.07x faster                                                  |
| mako                       | 11.9 ms                                                | 11.1 ms: 1.07x faster                                                  |
| chameleon                  | 7.41 ms                                                | 6.96 ms: 1.06x faster                                                  |
| crypto_pyaes               | 81.9 ms                                                | 77.0 ms: 1.06x faster                                                  |
| scimark_monte_carlo        | 75.1 ms                                                | 70.9 ms: 1.06x faster                                                  |
| float                      | 84.7 ms                                                | 80.0 ms: 1.06x faster                                                  |
| deepcopy                   | 371 us                                                 | 351 us: 1.06x faster                                                   |
| generators                 | 31.2 ms                                                | 29.5 ms: 1.06x faster                                                  |
| async_tree_none            | 472 ms                                                 | 447 ms: 1.06x faster                                                   |
| raytrace                   | 312 ms                                                 | 297 ms: 1.05x faster                                                   |
| pickle_pure_python         | 324 us                                                 | 308 us: 1.05x faster                                                   |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.82 ms: 1.05x faster                                                  |
| deepcopy_memo              | 40.7 us                                                | 38.9 us: 1.05x faster                                                  |
| chaos                      | 67.0 ms                                                | 64.0 ms: 1.05x faster                                                  |
| nbody                      | 97.0 ms                                                | 92.7 ms: 1.05x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 162 ms: 1.05x faster                                                   |
| sympy_str                  | 300 ms                                                 | 287 ms: 1.05x faster                                                   |
| fannkuch                   | 417 ms                                                 | 399 ms: 1.05x faster                                                   |
| tornado_http               | 103 ms                                                 | 99.0 ms: 1.04x faster                                                  |
| regex_compile              | 148 ms                                                 | 143 ms: 1.04x faster                                                   |
| pathlib                    | 19.3 ms                                                | 18.7 ms: 1.03x faster                                                  |
| unpickle                   | 15.9 us                                                | 15.4 us: 1.03x faster                                                  |
| coroutines                 | 23.2 ms                                                | 22.4 ms: 1.03x faster                                                  |
| sqlglot_parse              | 1.36 ms                                                | 1.32 ms: 1.03x faster                                                  |
| sqlglot_normalize          | 110 ms                                                 | 108 ms: 1.02x faster                                                   |
| logging_silent             | 104 ns                                                 | 102 ns: 1.02x faster                                                   |
| xml_etree_process          | 61.7 ms                                                | 60.6 ms: 1.02x faster                                                  |
| json_loads                 | 28.5 us                                                | 28.1 us: 1.01x faster                                                  |
| sqlglot_transpile          | 1.68 ms                                                | 1.66 ms: 1.01x faster                                                  |
| scimark_sor                | 129 ms                                                 | 127 ms: 1.01x faster                                                   |
| meteor_contest             | 112 ms                                                 | 111 ms: 1.01x faster                                                   |
| mdp                        | 2.63 sec                                               | 2.61 sec: 1.01x faster                                                 |
| xml_etree_generate         | 89.2 ms                                                | 88.6 ms: 1.01x faster                                                  |
| sympy_integrate            | 21.4 ms                                                | 21.3 ms: 1.01x faster                                                  |
| pickle_dict                | 35.5 us                                                | 35.4 us: 1.00x faster                                                  |
| docutils                   | 2.77 sec                                               | 2.78 sec: 1.00x slower                                                 |
| pidigits                   | 187 ms                                                 | 189 ms: 1.01x slower                                                   |
| async_generators           | 463 ms                                                 | 469 ms: 1.01x slower                                                   |
| sqlite_synth               | 2.83 us                                                | 2.87 us: 1.01x slower                                                  |
| richards                   | 45.8 ms                                                | 46.5 ms: 1.01x slower                                                  |
| sympy_expand               | 478 ms                                                 | 486 ms: 1.02x slower                                                   |
| xml_etree_iterparse        | 107 ms                                                 | 108 ms: 1.02x slower                                                   |
| json_dumps                 | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                  |
| pyflate                    | 482 ms                                                 | 493 ms: 1.02x slower                                                   |
| create_gc_cycles           | 1.48 ms                                                | 1.51 ms: 1.02x slower                                                  |
| dulwich_log                | 68.5 ms                                                | 70.0 ms: 1.02x slower                                                  |
| asyncio_websockets         | 551 ms                                                 | 564 ms: 1.02x slower                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 743 ms: 1.02x slower                                                   |
| async_tree_none_tg         | 450 ms                                                 | 461 ms: 1.03x slower                                                   |
| bench_thread_pool          | 842 us                                                 | 864 us: 1.03x slower                                                   |
| 2to3                       | 274 ms                                                 | 282 ms: 1.03x slower                                                   |
| pickle                     | 11.6 us                                                | 11.9 us: 1.03x slower                                                  |
| asyncio_tcp                | 491 ms                                                 | 505 ms: 1.03x slower                                                   |
| richards_super             | 51.5 ms                                                | 53.1 ms: 1.03x slower                                                  |
| sqlglot_optimize           | 54.8 ms                                                | 56.8 ms: 1.04x slower                                                  |
| unpickle_pure_python       | 230 us                                                 | 239 us: 1.04x slower                                                   |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.85 sec: 1.04x slower                                                 |
| async_tree_memoization_tg  | 575 ms                                                 | 597 ms: 1.04x slower                                                   |
| pickle_list                | 5.08 us                                                | 5.29 us: 1.04x slower                                                  |
| aiohttp                    | 1.15 ms                                                | 1.20 ms: 1.05x slower                                                  |
| gunicorn                   | 1.24 ms                                                | 1.30 ms: 1.05x slower                                                  |
| async_tree_io_tg           | 1.18 sec                                               | 1.24 sec: 1.05x slower                                                 |
| regex_effbot               | 3.61 ms                                                | 3.79 ms: 1.05x slower                                                  |
| async_tree_io              | 1.16 sec                                               | 1.22 sec: 1.05x slower                                                 |
| pycparser                  | 1.18 sec                                               | 1.26 sec: 1.07x slower                                                 |
| gc_traversal               | 3.79 ms                                                | 4.07 ms: 1.07x slower                                                  |
| nqueens                    | 83.3 ms                                                | 90.0 ms: 1.08x slower                                                  |
| scimark_lu                 | 118 ms                                                 | 129 ms: 1.10x slower                                                   |
| hexiom                     | 6.41 ms                                                | 7.06 ms: 1.10x slower                                                  |
| regex_dna                  | 212 ms                                                 | 234 ms: 1.10x slower                                                   |
| bench_mp_pool              | 24.0 ms                                                | 26.8 ms: 1.12x slower                                                  |
| regex_v8                   | 23.1 ms                                                | 25.9 ms: 1.12x slower                                                  |
| go                         | 139 ms                                                 | 157 ms: 1.13x slower                                                   |
| telco                      | 7.10 ms                                                | 8.43 ms: 1.19x slower                                                  |
| python_startup             | 9.55 ms                                                | 12.6 ms: 1.32x slower                                                  |
| coverage                   | 72.7 ms                                                | 98.5 ms: 1.35x slower                                                  |
| python_startup_no_site     | 6.94 ms                                                | 11.2 ms: 1.61x slower                                                  |
| unpack_sequence            | 54.0 ns                                                | 87.8 ns: 1.63x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (10): json, pprint_safe_repr, async_tree_memoization, spectral_norm, dask, django_template, xml_etree_parse, async_tree_cpu_io_mixed, pprint_pformat, mypy2
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240314-3.13.0a5+-61e54bf-JIT/bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 86.98% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.17x