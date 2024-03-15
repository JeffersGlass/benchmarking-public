# Results vs. 3.12.0

- fork: mdboom
- ref: estimate_too_short
- machine: linux-x86_64
- commit hash: c3a9b5a
- commit date: 2024-03-14
- overall geometric mean: 1.00x slower
- HPT reliability: 66.82%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.16x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 280 ms: 1.02x slower                                                 |
| chameleon      | 7.41 ms                                                | 7.00 ms: 1.06x faster                                                |
| docutils       | 2.77 sec                                               | 2.72 sec: 1.02x faster                                               |
| tornado_http   | 103 ms                                                 | 98.6 ms: 1.04x faster                                                |
| Geometric mean | (ref)                                                  | 1.02x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 445 ms: 1.06x faster                                                 |
| async_tree_none_tg         | 450 ms                                                 | 458 ms: 1.02x slower                                                 |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 740 ms: 1.02x slower                                                 |
| async_tree_memoization_tg  | 575 ms                                                 | 587 ms: 1.02x slower                                                 |
| async_tree_io_tg           | 1.18 sec                                               | 1.23 sec: 1.04x slower                                               |
| async_tree_io              | 1.16 sec                                               | 1.20 sec: 1.04x slower                                               |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                         |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 81.3 ms: 1.04x faster                                                |
| nbody          | 97.0 ms                                                | 93.1 ms: 1.04x faster                                                |
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                 |
| Geometric mean | (ref)                                                  | 1.02x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 142 ms: 1.04x faster                                                 |
| regex_dna      | 212 ms                                                 | 224 ms: 1.06x slower                                                 |
| regex_effbot   | 3.61 ms                                                | 3.83 ms: 1.06x slower                                                |
| regex_v8       | 23.1 ms                                                | 25.7 ms: 1.11x slower                                                |
| Geometric mean | (ref)                                                  | 1.05x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.05 sec: 1.13x faster                                               |
| unpickle_list        | 5.29 us                                                | 4.88 us: 1.08x faster                                                |
| pickle_pure_python   | 324 us                                                 | 304 us: 1.07x faster                                                 |
| unpickle             | 15.9 us                                                | 15.0 us: 1.06x faster                                                |
| xml_etree_process    | 61.7 ms                                                | 59.7 ms: 1.03x faster                                                |
| xml_etree_generate   | 89.2 ms                                                | 86.9 ms: 1.03x faster                                                |
| pickle_dict          | 35.5 us                                                | 34.6 us: 1.03x faster                                                |
| json_loads           | 28.5 us                                                | 28.1 us: 1.01x faster                                                |
| xml_etree_parse      | 159 ms                                                 | 159 ms: 1.00x faster                                                 |
| pickle_list          | 5.08 us                                                | 5.10 us: 1.00x slower                                                |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                |
| unpickle_pure_python | 230 us                                                 | 237 us: 1.03x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                         |

Benchmark hidden because not significant (2): xml_etree_iterparse, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.6 ms: 1.32x slower                                                |
| python_startup_no_site | 6.94 ms                                                | 11.2 ms: 1.61x slower                                                |
| Geometric mean         | (ref)                                                  | 1.46x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 10.9 ms: 1.10x faster                                                |
| django_template | 34.6 ms                                                | 33.9 ms: 1.02x faster                                                |
| Geometric mean  | (ref)                                                  | 1.06x faster                                                         |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 109 us: 1.45x faster                                                 |
| comprehensions             | 21.8 us                                                | 17.2 us: 1.27x faster                                                |
| tomli_loads                | 2.33 sec                                               | 2.05 sec: 1.13x faster                                               |
| deepcopy_reduce            | 3.35 us                                                | 3.01 us: 1.11x faster                                                |
| logging_format             | 7.23 us                                                | 6.53 us: 1.11x faster                                                |
| logging_simple             | 6.46 us                                                | 5.86 us: 1.10x faster                                                |
| scimark_fft                | 382 ms                                                 | 347 ms: 1.10x faster                                                 |
| mako                       | 11.9 ms                                                | 10.9 ms: 1.10x faster                                                |
| raytrace                   | 312 ms                                                 | 286 ms: 1.09x faster                                                 |
| deepcopy                   | 371 us                                                 | 342 us: 1.09x faster                                                 |
| deepcopy_memo              | 40.7 us                                                | 37.5 us: 1.09x faster                                                |
| crypto_pyaes               | 81.9 ms                                                | 75.5 ms: 1.08x faster                                                |
| unpickle_list              | 5.29 us                                                | 4.88 us: 1.08x faster                                                |
| pickle_pure_python         | 324 us                                                 | 304 us: 1.07x faster                                                 |
| scimark_monte_carlo        | 75.1 ms                                                | 70.7 ms: 1.06x faster                                                |
| async_tree_none            | 472 ms                                                 | 445 ms: 1.06x faster                                                 |
| unpickle                   | 15.9 us                                                | 15.0 us: 1.06x faster                                                |
| chameleon                  | 7.41 ms                                                | 7.00 ms: 1.06x faster                                                |
| sympy_str                  | 300 ms                                                 | 283 ms: 1.06x faster                                                 |
| gc_traversal               | 3.79 ms                                                | 3.59 ms: 1.06x faster                                                |
| generators                 | 31.2 ms                                                | 29.6 ms: 1.05x faster                                                |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.05x faster                                                 |
| chaos                      | 67.0 ms                                                | 63.6 ms: 1.05x faster                                                |
| pathlib                    | 19.3 ms                                                | 18.4 ms: 1.05x faster                                                |
| coroutines                 | 23.2 ms                                                | 22.0 ms: 1.05x faster                                                |
| regex_compile              | 148 ms                                                 | 142 ms: 1.04x faster                                                 |
| float                      | 84.7 ms                                                | 81.3 ms: 1.04x faster                                                |
| nbody                      | 97.0 ms                                                | 93.1 ms: 1.04x faster                                                |
| tornado_http               | 103 ms                                                 | 98.6 ms: 1.04x faster                                                |
| sqlglot_parse              | 1.36 ms                                                | 1.31 ms: 1.04x faster                                                |
| fannkuch                   | 417 ms                                                 | 401 ms: 1.04x faster                                                 |
| pprint_safe_repr           | 776 ms                                                 | 748 ms: 1.04x faster                                                 |
| xml_etree_process          | 61.7 ms                                                | 59.7 ms: 1.03x faster                                                |
| spectral_norm              | 115 ms                                                 | 111 ms: 1.03x faster                                                 |
| sqlglot_normalize          | 110 ms                                                 | 107 ms: 1.03x faster                                                 |
| logging_silent             | 104 ns                                                 | 102 ns: 1.03x faster                                                 |
| sympy_integrate            | 21.4 ms                                                | 20.8 ms: 1.03x faster                                                |
| sqlglot_transpile          | 1.68 ms                                                | 1.64 ms: 1.03x faster                                                |
| xml_etree_generate         | 89.2 ms                                                | 86.9 ms: 1.03x faster                                                |
| pickle_dict                | 35.5 us                                                | 34.6 us: 1.03x faster                                                |
| pprint_pformat             | 1.57 sec                                               | 1.53 sec: 1.02x faster                                               |
| json                       | 5.26 ms                                                | 5.14 ms: 1.02x faster                                                |
| django_template            | 34.6 ms                                                | 33.9 ms: 1.02x faster                                                |
| meteor_contest             | 112 ms                                                 | 110 ms: 1.02x faster                                                 |
| docutils                   | 2.77 sec                                               | 2.72 sec: 1.02x faster                                               |
| nqueens                    | 83.3 ms                                                | 81.8 ms: 1.02x faster                                                |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.99 ms: 1.01x faster                                                |
| json_loads                 | 28.5 us                                                | 28.1 us: 1.01x faster                                                |
| xml_etree_parse            | 159 ms                                                 | 159 ms: 1.00x faster                                                 |
| pickle_list                | 5.08 us                                                | 5.10 us: 1.00x slower                                                |
| deltablue                  | 3.72 ms                                                | 3.75 ms: 1.01x slower                                                |
| richards_super             | 51.5 ms                                                | 52.0 ms: 1.01x slower                                                |
| pidigits                   | 187 ms                                                 | 189 ms: 1.01x slower                                                 |
| sympy_expand               | 478 ms                                                 | 484 ms: 1.01x slower                                                 |
| async_generators           | 463 ms                                                 | 469 ms: 1.01x slower                                                 |
| dulwich_log                | 68.5 ms                                                | 69.4 ms: 1.01x slower                                                |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                |
| bench_thread_pool          | 842 us                                                 | 857 us: 1.02x slower                                                 |
| async_tree_none_tg         | 450 ms                                                 | 458 ms: 1.02x slower                                                 |
| pyflate                    | 482 ms                                                 | 492 ms: 1.02x slower                                                 |
| 2to3                       | 274 ms                                                 | 280 ms: 1.02x slower                                                 |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 740 ms: 1.02x slower                                                 |
| sqlite_synth               | 2.83 us                                                | 2.89 us: 1.02x slower                                                |
| async_tree_memoization_tg  | 575 ms                                                 | 587 ms: 1.02x slower                                                 |
| asyncio_websockets         | 551 ms                                                 | 563 ms: 1.02x slower                                                 |
| sqlglot_optimize           | 54.8 ms                                                | 56.2 ms: 1.02x slower                                                |
| pycparser                  | 1.18 sec                                               | 1.21 sec: 1.03x slower                                               |
| unpickle_pure_python       | 230 us                                                 | 237 us: 1.03x slower                                                 |
| create_gc_cycles           | 1.48 ms                                                | 1.52 ms: 1.03x slower                                                |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.85 sec: 1.03x slower                                               |
| async_tree_io_tg           | 1.18 sec                                               | 1.23 sec: 1.04x slower                                               |
| gunicorn                   | 1.24 ms                                                | 1.29 ms: 1.04x slower                                                |
| asyncio_tcp                | 491 ms                                                 | 510 ms: 1.04x slower                                                 |
| async_tree_io              | 1.16 sec                                               | 1.20 sec: 1.04x slower                                               |
| mdp                        | 2.63 sec                                               | 2.74 sec: 1.04x slower                                               |
| aiohttp                    | 1.15 ms                                                | 1.20 ms: 1.04x slower                                                |
| hexiom                     | 6.41 ms                                                | 6.74 ms: 1.05x slower                                                |
| regex_dna                  | 212 ms                                                 | 224 ms: 1.06x slower                                                 |
| regex_effbot               | 3.61 ms                                                | 3.83 ms: 1.06x slower                                                |
| scimark_sor                | 129 ms                                                 | 138 ms: 1.07x slower                                                 |
| bench_mp_pool              | 24.0 ms                                                | 26.4 ms: 1.10x slower                                                |
| scimark_lu                 | 118 ms                                                 | 130 ms: 1.10x slower                                                 |
| regex_v8                   | 23.1 ms                                                | 25.7 ms: 1.11x slower                                                |
| go                         | 139 ms                                                 | 156 ms: 1.12x slower                                                 |
| telco                      | 7.10 ms                                                | 8.33 ms: 1.17x slower                                                |
| python_startup             | 9.55 ms                                                | 12.6 ms: 1.32x slower                                                |
| coverage                   | 72.7 ms                                                | 96.0 ms: 1.32x slower                                                |
| python_startup_no_site     | 6.94 ms                                                | 11.2 ms: 1.61x slower                                                |
| unpack_sequence            | 54.0 ns                                                | 92.9 ns: 1.72x slower                                                |
| Geometric mean             | (ref)                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (7): async_tree_memoization, async_tree_cpu_io_mixed, xml_etree_iterparse, pickle, richards, dask, mypy2
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240314-3.13.0a5+-c3a9b5a-JIT/bm-20240314-linux-x86_64-mdboom-estimate_too_short-3.13.0a5+-c3a9b5a.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 66.82% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.16x