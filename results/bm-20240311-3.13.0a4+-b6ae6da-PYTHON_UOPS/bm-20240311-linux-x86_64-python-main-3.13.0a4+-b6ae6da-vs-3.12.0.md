# Results vs. 3.12.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: b6ae6da
- commit date: 2024-03-11
- overall geometric mean: 1.06x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 297 ms: 1.08x slower                                   |
| chameleon      | 7.41 ms                                                | 7.13 ms: 1.04x faster                                  |
| docutils       | 2.77 sec                                               | 2.86 sec: 1.03x slower                                 |
| Geometric mean | (ref)                                                  | 1.02x slower                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 459 ms: 1.03x faster                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 743 ms: 1.02x slower                                   |
| async_tree_memoization     | 578 ms                                                 | 593 ms: 1.03x slower                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 755 ms: 1.04x slower                                   |
| async_tree_none_tg         | 450 ms                                                 | 472 ms: 1.05x slower                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 608 ms: 1.06x slower                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.26 sec: 1.06x slower                                 |
| async_tree_io              | 1.16 sec                                               | 1.23 sec: 1.07x slower                                 |
| Geometric mean             | (ref)                                                  | 1.04x slower                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 191 ms: 1.02x slower                                   |
| float          | 84.7 ms                                                | 93.0 ms: 1.10x slower                                  |
| nbody          | 97.0 ms                                                | 120 ms: 1.24x slower                                   |
| Geometric mean | (ref)                                                  | 1.11x slower                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.59 ms: 1.00x faster                                  |
| regex_dna      | 212 ms                                                 | 216 ms: 1.02x slower                                   |
| regex_v8       | 23.1 ms                                                | 25.1 ms: 1.08x slower                                  |
| regex_compile  | 148 ms                                                 | 174 ms: 1.17x slower                                   |
| Geometric mean | (ref)                                                  | 1.07x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| unpickle_list        | 5.29 us                                                | 4.88 us: 1.08x faster                                  |
| pickle_dict          | 35.5 us                                                | 32.9 us: 1.08x faster                                  |
| pickle_pure_python   | 324 us                                                 | 310 us: 1.05x faster                                   |
| pickle_list          | 5.08 us                                                | 4.90 us: 1.04x faster                                  |
| unpickle             | 15.9 us                                                | 15.3 us: 1.04x faster                                  |
| json_loads           | 28.5 us                                                | 28.2 us: 1.01x faster                                  |
| xml_etree_process    | 61.7 ms                                                | 62.3 ms: 1.01x slower                                  |
| xml_etree_generate   | 89.2 ms                                                | 90.8 ms: 1.02x slower                                  |
| json_dumps           | 10.4 ms                                                | 10.6 ms: 1.02x slower                                  |
| pickle               | 11.6 us                                                | 12.0 us: 1.04x slower                                  |
| tomli_loads          | 2.33 sec                                               | 2.43 sec: 1.04x slower                                 |
| xml_etree_iterparse  | 107 ms                                                 | 112 ms: 1.05x slower                                   |
| unpickle_pure_python | 230 us                                                 | 269 us: 1.17x slower                                   |
| Geometric mean       | (ref)                                                  | 1.00x slower                                           |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.4 ms: 1.09x slower                                  |
| python_startup_no_site | 6.94 ms                                                | 9.01 ms: 1.30x slower                                  |
| Geometric mean         | (ref)                                                  | 1.19x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 34.6 ms                                                | 35.3 ms: 1.02x slower                                  |
| mako            | 11.9 ms                                                | 12.7 ms: 1.07x slower                                  |
| Geometric mean  | (ref)                                                  | 1.05x slower                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 119 us: 1.33x faster                                   |
| unpickle_list              | 5.29 us                                                | 4.88 us: 1.08x faster                                  |
| pickle_dict                | 35.5 us                                                | 32.9 us: 1.08x faster                                  |
| comprehensions             | 21.8 us                                                | 20.7 us: 1.05x faster                                  |
| deepcopy_reduce            | 3.35 us                                                | 3.18 us: 1.05x faster                                  |
| pickle_pure_python         | 324 us                                                 | 310 us: 1.05x faster                                   |
| generators                 | 31.2 ms                                                | 30.0 ms: 1.04x faster                                  |
| chameleon                  | 7.41 ms                                                | 7.13 ms: 1.04x faster                                  |
| pickle_list                | 5.08 us                                                | 4.90 us: 1.04x faster                                  |
| unpickle                   | 15.9 us                                                | 15.3 us: 1.04x faster                                  |
| coroutines                 | 23.2 ms                                                | 22.5 ms: 1.03x faster                                  |
| async_tree_none            | 472 ms                                                 | 459 ms: 1.03x faster                                   |
| logging_format             | 7.23 us                                                | 7.08 us: 1.02x faster                                  |
| logging_simple             | 6.46 us                                                | 6.33 us: 1.02x faster                                  |
| deepcopy                   | 371 us                                                 | 367 us: 1.01x faster                                   |
| sympy_sum                  | 169 ms                                                 | 167 ms: 1.01x faster                                   |
| json_loads                 | 28.5 us                                                | 28.2 us: 1.01x faster                                  |
| regex_effbot               | 3.61 ms                                                | 3.59 ms: 1.00x faster                                  |
| sympy_integrate            | 21.4 ms                                                | 21.5 ms: 1.00x slower                                  |
| xml_etree_process          | 61.7 ms                                                | 62.3 ms: 1.01x slower                                  |
| sympy_str                  | 300 ms                                                 | 303 ms: 1.01x slower                                   |
| async_generators           | 463 ms                                                 | 469 ms: 1.01x slower                                   |
| dask                       | 372 ms                                                 | 378 ms: 1.02x slower                                   |
| xml_etree_generate         | 89.2 ms                                                | 90.8 ms: 1.02x slower                                  |
| regex_dna                  | 212 ms                                                 | 216 ms: 1.02x slower                                   |
| django_template            | 34.6 ms                                                | 35.3 ms: 1.02x slower                                  |
| pidigits                   | 187 ms                                                 | 191 ms: 1.02x slower                                   |
| json_dumps                 | 10.4 ms                                                | 10.6 ms: 1.02x slower                                  |
| asyncio_websockets         | 551 ms                                                 | 564 ms: 1.02x slower                                   |
| sqlglot_normalize          | 110 ms                                                 | 113 ms: 1.02x slower                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 743 ms: 1.02x slower                                   |
| async_tree_memoization     | 578 ms                                                 | 593 ms: 1.03x slower                                   |
| deltablue                  | 3.72 ms                                                | 3.82 ms: 1.03x slower                                  |
| docutils                   | 2.77 sec                                               | 2.86 sec: 1.03x slower                                 |
| mdp                        | 2.63 sec                                               | 2.72 sec: 1.03x slower                                 |
| asyncio_tcp                | 491 ms                                                 | 507 ms: 1.03x slower                                   |
| bench_thread_pool          | 842 us                                                 | 872 us: 1.04x slower                                   |
| pickle                     | 11.6 us                                                | 12.0 us: 1.04x slower                                  |
| gc_traversal               | 3.79 ms                                                | 3.94 ms: 1.04x slower                                  |
| deepcopy_memo              | 40.7 us                                                | 42.3 us: 1.04x slower                                  |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 755 ms: 1.04x slower                                   |
| meteor_contest             | 112 ms                                                 | 117 ms: 1.04x slower                                   |
| tomli_loads                | 2.33 sec                                               | 2.43 sec: 1.04x slower                                 |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.86 sec: 1.04x slower                                 |
| xml_etree_iterparse        | 107 ms                                                 | 112 ms: 1.05x slower                                   |
| sqlite_synth               | 2.83 us                                                | 2.96 us: 1.05x slower                                  |
| create_gc_cycles           | 1.48 ms                                                | 1.54 ms: 1.05x slower                                  |
| async_tree_none_tg         | 450 ms                                                 | 472 ms: 1.05x slower                                   |
| aiohttp                    | 1.15 ms                                                | 1.21 ms: 1.05x slower                                  |
| sqlglot_parse              | 1.36 ms                                                | 1.44 ms: 1.06x slower                                  |
| crypto_pyaes               | 81.9 ms                                                | 86.5 ms: 1.06x slower                                  |
| unpack_sequence            | 54.0 ns                                                | 57.0 ns: 1.06x slower                                  |
| async_tree_memoization_tg  | 575 ms                                                 | 608 ms: 1.06x slower                                   |
| sqlglot_transpile          | 1.68 ms                                                | 1.78 ms: 1.06x slower                                  |
| gunicorn                   | 1.24 ms                                                | 1.31 ms: 1.06x slower                                  |
| async_tree_io_tg           | 1.18 sec                                               | 1.26 sec: 1.06x slower                                 |
| dulwich_log                | 68.5 ms                                                | 73.1 ms: 1.07x slower                                  |
| async_tree_io              | 1.16 sec                                               | 1.23 sec: 1.07x slower                                 |
| mako                       | 11.9 ms                                                | 12.7 ms: 1.07x slower                                  |
| sympy_expand               | 478 ms                                                 | 512 ms: 1.07x slower                                   |
| regex_v8                   | 23.1 ms                                                | 25.1 ms: 1.08x slower                                  |
| 2to3                       | 274 ms                                                 | 297 ms: 1.08x slower                                   |
| python_startup             | 9.55 ms                                                | 10.4 ms: 1.09x slower                                  |
| raytrace                   | 312 ms                                                 | 342 ms: 1.09x slower                                   |
| pycparser                  | 1.18 sec                                               | 1.29 sec: 1.10x slower                                 |
| float                      | 84.7 ms                                                | 93.0 ms: 1.10x slower                                  |
| scimark_monte_carlo        | 75.1 ms                                                | 82.6 ms: 1.10x slower                                  |
| mypy2                      | 830 ms                                                 | 918 ms: 1.11x slower                                   |
| pprint_safe_repr           | 776 ms                                                 | 860 ms: 1.11x slower                                   |
| sqlglot_optimize           | 54.8 ms                                                | 61.0 ms: 1.11x slower                                  |
| chaos                      | 67.0 ms                                                | 74.9 ms: 1.12x slower                                  |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.69 ms: 1.13x slower                                  |
| fannkuch                   | 417 ms                                                 | 472 ms: 1.13x slower                                   |
| scimark_fft                | 382 ms                                                 | 436 ms: 1.14x slower                                   |
| pprint_pformat             | 1.57 sec                                               | 1.79 sec: 1.14x slower                                 |
| scimark_sor                | 129 ms                                                 | 150 ms: 1.16x slower                                   |
| pyflate                    | 482 ms                                                 | 564 ms: 1.17x slower                                   |
| unpickle_pure_python       | 230 us                                                 | 269 us: 1.17x slower                                   |
| regex_compile              | 148 ms                                                 | 174 ms: 1.17x slower                                   |
| nqueens                    | 83.3 ms                                                | 99.1 ms: 1.19x slower                                  |
| richards_super             | 51.5 ms                                                | 61.8 ms: 1.20x slower                                  |
| richards                   | 45.8 ms                                                | 55.6 ms: 1.21x slower                                  |
| telco                      | 7.10 ms                                                | 8.66 ms: 1.22x slower                                  |
| spectral_norm              | 115 ms                                                 | 141 ms: 1.23x slower                                   |
| nbody                      | 97.0 ms                                                | 120 ms: 1.24x slower                                   |
| go                         | 139 ms                                                 | 176 ms: 1.26x slower                                   |
| python_startup_no_site     | 6.94 ms                                                | 9.01 ms: 1.30x slower                                  |
| scimark_lu                 | 118 ms                                                 | 158 ms: 1.34x slower                                   |
| coverage                   | 72.7 ms                                                | 97.4 ms: 1.34x slower                                  |
| hexiom                     | 6.41 ms                                                | 8.79 ms: 1.37x slower                                  |
| Geometric mean             | (ref)                                                  | 1.06x slower                                           |

Benchmark hidden because not significant (6): json, xml_etree_parse, bench_mp_pool, logging_silent, tornado_http, pathlib
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240311-3.13.0a4+-b6ae6da-PYTHON_UOPS/bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 0.94x