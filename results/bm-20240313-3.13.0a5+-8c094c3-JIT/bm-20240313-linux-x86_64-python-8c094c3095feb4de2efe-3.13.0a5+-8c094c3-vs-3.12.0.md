# Results vs. 3.12.0

- fork: python
- ref: 8c094c3095feb4de2efe
- machine: linux-x86_64
- commit hash: 8c094c3
- commit date: 2024-03-13
- overall geometric mean: 1.01x slower
- HPT reliability: 96.45%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 282 ms: 1.03x slower                                                   |
| chameleon      | 7.41 ms                                                | 6.90 ms: 1.07x faster                                                  |
| tornado_http   | 103 ms                                                 | 98.7 ms: 1.04x faster                                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 449 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 740 ms: 1.02x slower                                                   |
| async_tree_none_tg         | 450 ms                                                 | 459 ms: 1.02x slower                                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 592 ms: 1.03x slower                                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.24 sec: 1.04x slower                                                 |
| async_tree_io              | 1.16 sec                                               | 1.22 sec: 1.05x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 79.8 ms: 1.06x faster                                                  |
| nbody          | 97.0 ms                                                | 92.4 ms: 1.05x faster                                                  |
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                   |
| Geometric mean | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 144 ms: 1.03x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.82 ms: 1.06x slower                                                  |
| regex_v8       | 23.1 ms                                                | 25.4 ms: 1.10x slower                                                  |
| regex_dna      | 212 ms                                                 | 238 ms: 1.12x slower                                                   |
| Geometric mean | (ref)                                                  | 1.06x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.08 sec: 1.12x faster                                                 |
| pickle_pure_python   | 324 us                                                 | 302 us: 1.07x faster                                                   |
| unpickle_list        | 5.29 us                                                | 4.93 us: 1.07x faster                                                  |
| unpickle             | 15.9 us                                                | 15.1 us: 1.05x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 59.9 ms: 1.03x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 86.8 ms: 1.03x faster                                                  |
| json_loads           | 28.5 us                                                | 27.9 us: 1.02x faster                                                  |
| pickle_dict          | 35.5 us                                                | 35.4 us: 1.00x faster                                                  |
| json_dumps           | 10.4 ms                                                | 10.4 ms: 1.00x slower                                                  |
| pickle               | 11.6 us                                                | 12.0 us: 1.03x slower                                                  |
| unpickle_pure_python | 230 us                                                 | 239 us: 1.04x slower                                                   |
| pickle_list          | 5.08 us                                                | 5.31 us: 1.04x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (2): xml_etree_parse, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.6 ms: 1.32x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 11.2 ms: 1.61x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.46x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 10.7 ms: 1.11x faster                                                  |
| django_template | 34.6 ms                                                | 34.4 ms: 1.01x faster                                                  |
| Geometric mean  | (ref)                                                  | 1.06x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 110 us: 1.43x faster                                                   |
| comprehensions             | 21.8 us                                                | 17.3 us: 1.26x faster                                                  |
| tomli_loads                | 2.33 sec                                               | 2.08 sec: 1.12x faster                                                 |
| logging_format             | 7.23 us                                                | 6.46 us: 1.12x faster                                                  |
| scimark_fft                | 382 ms                                                 | 343 ms: 1.11x faster                                                   |
| mako                       | 11.9 ms                                                | 10.7 ms: 1.11x faster                                                  |
| logging_simple             | 6.46 us                                                | 5.86 us: 1.10x faster                                                  |
| crypto_pyaes               | 81.9 ms                                                | 75.6 ms: 1.08x faster                                                  |
| deepcopy_reduce            | 3.35 us                                                | 3.09 us: 1.08x faster                                                  |
| deltablue                  | 3.72 ms                                                | 3.44 ms: 1.08x faster                                                  |
| pickle_pure_python         | 324 us                                                 | 302 us: 1.07x faster                                                   |
| chameleon                  | 7.41 ms                                                | 6.90 ms: 1.07x faster                                                  |
| unpickle_list              | 5.29 us                                                | 4.93 us: 1.07x faster                                                  |
| scimark_monte_carlo        | 75.1 ms                                                | 70.1 ms: 1.07x faster                                                  |
| raytrace                   | 312 ms                                                 | 294 ms: 1.06x faster                                                   |
| float                      | 84.7 ms                                                | 79.8 ms: 1.06x faster                                                  |
| fannkuch                   | 417 ms                                                 | 395 ms: 1.06x faster                                                   |
| async_tree_none            | 472 ms                                                 | 449 ms: 1.05x faster                                                   |
| generators                 | 31.2 ms                                                | 29.7 ms: 1.05x faster                                                  |
| nbody                      | 97.0 ms                                                | 92.4 ms: 1.05x faster                                                  |
| deepcopy                   | 371 us                                                 | 354 us: 1.05x faster                                                   |
| unpickle                   | 15.9 us                                                | 15.1 us: 1.05x faster                                                  |
| chaos                      | 67.0 ms                                                | 64.1 ms: 1.04x faster                                                  |
| sympy_str                  | 300 ms                                                 | 288 ms: 1.04x faster                                                   |
| tornado_http               | 103 ms                                                 | 98.7 ms: 1.04x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 163 ms: 1.04x faster                                                   |
| sqlglot_parse              | 1.36 ms                                                | 1.31 ms: 1.04x faster                                                  |
| regex_compile              | 148 ms                                                 | 144 ms: 1.03x faster                                                   |
| deepcopy_memo              | 40.7 us                                                | 39.5 us: 1.03x faster                                                  |
| xml_etree_process          | 61.7 ms                                                | 59.9 ms: 1.03x faster                                                  |
| pathlib                    | 19.3 ms                                                | 18.8 ms: 1.03x faster                                                  |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.91 ms: 1.03x faster                                                  |
| logging_silent             | 104 ns                                                 | 102 ns: 1.03x faster                                                   |
| xml_etree_generate         | 89.2 ms                                                | 86.8 ms: 1.03x faster                                                  |
| json_loads                 | 28.5 us                                                | 27.9 us: 1.02x faster                                                  |
| meteor_contest             | 112 ms                                                 | 110 ms: 1.02x faster                                                   |
| json                       | 5.26 ms                                                | 5.16 ms: 1.02x faster                                                  |
| coroutines                 | 23.2 ms                                                | 22.7 ms: 1.02x faster                                                  |
| sqlglot_transpile          | 1.68 ms                                                | 1.66 ms: 1.02x faster                                                  |
| sqlglot_normalize          | 110 ms                                                 | 108 ms: 1.02x faster                                                   |
| sympy_integrate            | 21.4 ms                                                | 21.2 ms: 1.01x faster                                                  |
| django_template            | 34.6 ms                                                | 34.4 ms: 1.01x faster                                                  |
| pickle_dict                | 35.5 us                                                | 35.4 us: 1.00x faster                                                  |
| json_dumps                 | 10.4 ms                                                | 10.4 ms: 1.00x slower                                                  |
| pprint_pformat             | 1.57 sec                                               | 1.58 sec: 1.01x slower                                                 |
| pidigits                   | 187 ms                                                 | 189 ms: 1.01x slower                                                   |
| richards_super             | 51.5 ms                                                | 52.2 ms: 1.01x slower                                                  |
| async_generators           | 463 ms                                                 | 469 ms: 1.01x slower                                                   |
| richards                   | 45.8 ms                                                | 46.5 ms: 1.01x slower                                                  |
| pyflate                    | 482 ms                                                 | 490 ms: 1.02x slower                                                   |
| sympy_expand               | 478 ms                                                 | 487 ms: 1.02x slower                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 740 ms: 1.02x slower                                                   |
| asyncio_websockets         | 551 ms                                                 | 563 ms: 1.02x slower                                                   |
| async_tree_none_tg         | 450 ms                                                 | 459 ms: 1.02x slower                                                   |
| bench_thread_pool          | 842 us                                                 | 862 us: 1.02x slower                                                   |
| spectral_norm              | 115 ms                                                 | 118 ms: 1.02x slower                                                   |
| asyncio_tcp                | 491 ms                                                 | 503 ms: 1.03x slower                                                   |
| create_gc_cycles           | 1.48 ms                                                | 1.52 ms: 1.03x slower                                                  |
| 2to3                       | 274 ms                                                 | 282 ms: 1.03x slower                                                   |
| dulwich_log                | 68.5 ms                                                | 70.5 ms: 1.03x slower                                                  |
| async_tree_memoization_tg  | 575 ms                                                 | 592 ms: 1.03x slower                                                   |
| pickle                     | 11.6 us                                                | 12.0 us: 1.03x slower                                                  |
| sqlglot_optimize           | 54.8 ms                                                | 56.6 ms: 1.03x slower                                                  |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.85 sec: 1.04x slower                                                 |
| unpickle_pure_python       | 230 us                                                 | 239 us: 1.04x slower                                                   |
| gc_traversal               | 3.79 ms                                                | 3.95 ms: 1.04x slower                                                  |
| gunicorn                   | 1.24 ms                                                | 1.30 ms: 1.04x slower                                                  |
| pickle_list                | 5.08 us                                                | 5.31 us: 1.04x slower                                                  |
| aiohttp                    | 1.15 ms                                                | 1.20 ms: 1.04x slower                                                  |
| async_tree_io_tg           | 1.18 sec                                               | 1.24 sec: 1.04x slower                                                 |
| mdp                        | 2.63 sec                                               | 2.75 sec: 1.04x slower                                                 |
| async_tree_io              | 1.16 sec                                               | 1.22 sec: 1.05x slower                                                 |
| regex_effbot               | 3.61 ms                                                | 3.82 ms: 1.06x slower                                                  |
| pycparser                  | 1.18 sec                                               | 1.25 sec: 1.06x slower                                                 |
| nqueens                    | 83.3 ms                                                | 90.5 ms: 1.09x slower                                                  |
| regex_v8                   | 23.1 ms                                                | 25.4 ms: 1.10x slower                                                  |
| bench_mp_pool              | 24.0 ms                                                | 26.4 ms: 1.10x slower                                                  |
| hexiom                     | 6.41 ms                                                | 7.09 ms: 1.11x slower                                                  |
| scimark_lu                 | 118 ms                                                 | 132 ms: 1.12x slower                                                   |
| regex_dna                  | 212 ms                                                 | 238 ms: 1.12x slower                                                   |
| go                         | 139 ms                                                 | 158 ms: 1.13x slower                                                   |
| telco                      | 7.10 ms                                                | 8.42 ms: 1.19x slower                                                  |
| python_startup             | 9.55 ms                                                | 12.6 ms: 1.32x slower                                                  |
| coverage                   | 72.7 ms                                                | 97.6 ms: 1.34x slower                                                  |
| python_startup_no_site     | 6.94 ms                                                | 11.2 ms: 1.61x slower                                                  |
| unpack_sequence            | 54.0 ns                                                | 90.6 ns: 1.68x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (10): async_tree_cpu_io_mixed, async_tree_memoization, xml_etree_parse, sqlite_synth, docutils, scimark_sor, pprint_safe_repr, xml_etree_iterparse, dask, mypy2
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240313-3.13.0a5+-8c094c3-JIT/bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 96.45% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.17x