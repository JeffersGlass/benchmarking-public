# Results vs. 3.12.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 8c094c3
- commit date: 2024-03-13
- overall geometric mean: 1.06x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 298 ms: 1.09x slower                                   |
| chameleon      | 7.41 ms                                                | 6.87 ms: 1.08x faster                                  |
| docutils       | 2.77 sec                                               | 2.87 sec: 1.04x slower                                 |
| tornado_http   | 103 ms                                                 | 104 ms: 1.01x slower                                   |
| Geometric mean | (ref)                                                  | 1.01x slower                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 463 ms: 1.02x faster                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 745 ms: 1.03x slower                                   |
| async_tree_memoization     | 578 ms                                                 | 594 ms: 1.03x slower                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 758 ms: 1.04x slower                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 601 ms: 1.05x slower                                   |
| async_tree_none_tg         | 450 ms                                                 | 473 ms: 1.05x slower                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.26 sec: 1.07x slower                                 |
| async_tree_io              | 1.16 sec                                               | 1.25 sec: 1.08x slower                                 |
| Geometric mean             | (ref)                                                  | 1.04x slower                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 192 ms: 1.02x slower                                   |
| float          | 84.7 ms                                                | 94.8 ms: 1.12x slower                                  |
| nbody          | 97.0 ms                                                | 122 ms: 1.25x slower                                   |
| Geometric mean | (ref)                                                  | 1.13x slower                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.59 ms: 1.00x faster                                  |
| regex_dna      | 212 ms                                                 | 229 ms: 1.08x slower                                   |
| regex_v8       | 23.1 ms                                                | 25.6 ms: 1.11x slower                                  |
| regex_compile  | 148 ms                                                 | 177 ms: 1.19x slower                                   |
| Geometric mean | (ref)                                                  | 1.09x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| unpickle_list        | 5.29 us                                                | 4.91 us: 1.08x faster                                  |
| pickle_dict          | 35.5 us                                                | 33.5 us: 1.06x faster                                  |
| pickle_pure_python   | 324 us                                                 | 306 us: 1.06x faster                                   |
| unpickle             | 15.9 us                                                | 15.1 us: 1.05x faster                                  |
| pickle_list          | 5.08 us                                                | 4.97 us: 1.02x faster                                  |
| pickle               | 11.6 us                                                | 11.5 us: 1.01x faster                                  |
| json_loads           | 28.5 us                                                | 28.3 us: 1.01x faster                                  |
| xml_etree_process    | 61.7 ms                                                | 62.2 ms: 1.01x slower                                  |
| xml_etree_parse      | 159 ms                                                 | 161 ms: 1.01x slower                                   |
| xml_etree_generate   | 89.2 ms                                                | 90.7 ms: 1.02x slower                                  |
| json_dumps           | 10.4 ms                                                | 10.6 ms: 1.02x slower                                  |
| xml_etree_iterparse  | 107 ms                                                 | 111 ms: 1.04x slower                                   |
| tomli_loads          | 2.33 sec                                               | 2.51 sec: 1.08x slower                                 |
| unpickle_pure_python | 230 us                                                 | 274 us: 1.19x slower                                   |
| Geometric mean       | (ref)                                                  | 1.01x slower                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.4 ms: 1.09x slower                                  |
| python_startup_no_site | 6.94 ms                                                | 8.99 ms: 1.30x slower                                  |
| Geometric mean         | (ref)                                                  | 1.19x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako           | 11.9 ms                                                | 12.6 ms: 1.06x slower                                  |
| Geometric mean | (ref)                                                  | 1.03x slower                                           |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 116 us: 1.36x faster                                   |
| deepcopy_reduce            | 3.35 us                                                | 3.09 us: 1.08x faster                                  |
| chameleon                  | 7.41 ms                                                | 6.87 ms: 1.08x faster                                  |
| unpickle_list              | 5.29 us                                                | 4.91 us: 1.08x faster                                  |
| pickle_dict                | 35.5 us                                                | 33.5 us: 1.06x faster                                  |
| pickle_pure_python         | 324 us                                                 | 306 us: 1.06x faster                                   |
| unpickle                   | 15.9 us                                                | 15.1 us: 1.05x faster                                  |
| coroutines                 | 23.2 ms                                                | 22.3 ms: 1.04x faster                                  |
| pickle_list                | 5.08 us                                                | 4.97 us: 1.02x faster                                  |
| logging_simple             | 6.46 us                                                | 6.32 us: 1.02x faster                                  |
| deepcopy                   | 371 us                                                 | 364 us: 1.02x faster                                   |
| logging_format             | 7.23 us                                                | 7.09 us: 1.02x faster                                  |
| comprehensions             | 21.8 us                                                | 21.4 us: 1.02x faster                                  |
| async_tree_none            | 472 ms                                                 | 463 ms: 1.02x faster                                   |
| pickle                     | 11.6 us                                                | 11.5 us: 1.01x faster                                  |
| generators                 | 31.2 ms                                                | 30.9 ms: 1.01x faster                                  |
| json_loads                 | 28.5 us                                                | 28.3 us: 1.01x faster                                  |
| regex_effbot               | 3.61 ms                                                | 3.59 ms: 1.00x faster                                  |
| xml_etree_process          | 61.7 ms                                                | 62.2 ms: 1.01x slower                                  |
| sympy_integrate            | 21.4 ms                                                | 21.7 ms: 1.01x slower                                  |
| xml_etree_parse            | 159 ms                                                 | 161 ms: 1.01x slower                                   |
| tornado_http               | 103 ms                                                 | 104 ms: 1.01x slower                                   |
| dask                       | 372 ms                                                 | 378 ms: 1.02x slower                                   |
| xml_etree_generate         | 89.2 ms                                                | 90.7 ms: 1.02x slower                                  |
| async_generators           | 463 ms                                                 | 472 ms: 1.02x slower                                   |
| json_dumps                 | 10.4 ms                                                | 10.6 ms: 1.02x slower                                  |
| sqlite_synth               | 2.83 us                                                | 2.89 us: 1.02x slower                                  |
| deltablue                  | 3.72 ms                                                | 3.80 ms: 1.02x slower                                  |
| asyncio_websockets         | 551 ms                                                 | 564 ms: 1.02x slower                                   |
| pidigits                   | 187 ms                                                 | 192 ms: 1.02x slower                                   |
| sympy_str                  | 300 ms                                                 | 307 ms: 1.02x slower                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 745 ms: 1.03x slower                                   |
| deepcopy_memo              | 40.7 us                                                | 41.9 us: 1.03x slower                                  |
| async_tree_memoization     | 578 ms                                                 | 594 ms: 1.03x slower                                   |
| create_gc_cycles           | 1.48 ms                                                | 1.52 ms: 1.03x slower                                  |
| sqlglot_normalize          | 110 ms                                                 | 114 ms: 1.03x slower                                   |
| asyncio_tcp                | 491 ms                                                 | 507 ms: 1.03x slower                                   |
| docutils                   | 2.77 sec                                               | 2.87 sec: 1.04x slower                                 |
| xml_etree_iterparse        | 107 ms                                                 | 111 ms: 1.04x slower                                   |
| bench_thread_pool          | 842 us                                                 | 876 us: 1.04x slower                                   |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.86 sec: 1.04x slower                                 |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 758 ms: 1.04x slower                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 601 ms: 1.05x slower                                   |
| async_tree_none_tg         | 450 ms                                                 | 473 ms: 1.05x slower                                   |
| sqlglot_parse              | 1.36 ms                                                | 1.44 ms: 1.06x slower                                  |
| gunicorn                   | 1.24 ms                                                | 1.32 ms: 1.06x slower                                  |
| mako                       | 11.9 ms                                                | 12.6 ms: 1.06x slower                                  |
| meteor_contest             | 112 ms                                                 | 119 ms: 1.06x slower                                   |
| sqlglot_transpile          | 1.68 ms                                                | 1.79 ms: 1.06x slower                                  |
| dulwich_log                | 68.5 ms                                                | 73.0 ms: 1.06x slower                                  |
| gc_traversal               | 3.79 ms                                                | 4.05 ms: 1.07x slower                                  |
| aiohttp                    | 1.15 ms                                                | 1.23 ms: 1.07x slower                                  |
| async_tree_io_tg           | 1.18 sec                                               | 1.26 sec: 1.07x slower                                 |
| crypto_pyaes               | 81.9 ms                                                | 87.7 ms: 1.07x slower                                  |
| mdp                        | 2.63 sec                                               | 2.83 sec: 1.07x slower                                 |
| tomli_loads                | 2.33 sec                                               | 2.51 sec: 1.08x slower                                 |
| async_tree_io              | 1.16 sec                                               | 1.25 sec: 1.08x slower                                 |
| regex_dna                  | 212 ms                                                 | 229 ms: 1.08x slower                                   |
| sympy_expand               | 478 ms                                                 | 519 ms: 1.09x slower                                   |
| 2to3                       | 274 ms                                                 | 298 ms: 1.09x slower                                   |
| python_startup             | 9.55 ms                                                | 10.4 ms: 1.09x slower                                  |
| scimark_sor                | 129 ms                                                 | 142 ms: 1.10x slower                                   |
| raytrace                   | 312 ms                                                 | 345 ms: 1.11x slower                                   |
| mypy2                      | 830 ms                                                 | 918 ms: 1.11x slower                                   |
| regex_v8                   | 23.1 ms                                                | 25.6 ms: 1.11x slower                                  |
| sqlglot_optimize           | 54.8 ms                                                | 61.2 ms: 1.12x slower                                  |
| float                      | 84.7 ms                                                | 94.8 ms: 1.12x slower                                  |
| chaos                      | 67.0 ms                                                | 75.3 ms: 1.12x slower                                  |
| pprint_safe_repr           | 776 ms                                                 | 873 ms: 1.13x slower                                   |
| scimark_fft                | 382 ms                                                 | 432 ms: 1.13x slower                                   |
| scimark_monte_carlo        | 75.1 ms                                                | 85.4 ms: 1.14x slower                                  |
| pycparser                  | 1.18 sec                                               | 1.35 sec: 1.15x slower                                 |
| fannkuch                   | 417 ms                                                 | 481 ms: 1.15x slower                                   |
| pprint_pformat             | 1.57 sec                                               | 1.83 sec: 1.17x slower                                 |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.92 ms: 1.17x slower                                  |
| regex_compile              | 148 ms                                                 | 177 ms: 1.19x slower                                   |
| unpickle_pure_python       | 230 us                                                 | 274 us: 1.19x slower                                   |
| pyflate                    | 482 ms                                                 | 590 ms: 1.22x slower                                   |
| richards_super             | 51.5 ms                                                | 63.4 ms: 1.23x slower                                  |
| richards                   | 45.8 ms                                                | 56.9 ms: 1.24x slower                                  |
| spectral_norm              | 115 ms                                                 | 143 ms: 1.24x slower                                   |
| nqueens                    | 83.3 ms                                                | 104 ms: 1.25x slower                                   |
| nbody                      | 97.0 ms                                                | 122 ms: 1.25x slower                                   |
| telco                      | 7.10 ms                                                | 8.91 ms: 1.26x slower                                  |
| go                         | 139 ms                                                 | 178 ms: 1.28x slower                                   |
| python_startup_no_site     | 6.94 ms                                                | 8.99 ms: 1.30x slower                                  |
| scimark_lu                 | 118 ms                                                 | 158 ms: 1.34x slower                                   |
| coverage                   | 72.7 ms                                                | 97.5 ms: 1.34x slower                                  |
| hexiom                     | 6.41 ms                                                | 9.14 ms: 1.43x slower                                  |
| Geometric mean             | (ref)                                                  | 1.06x slower                                           |

Benchmark hidden because not significant (7): json, django_template, bench_mp_pool, sympy_sum, unpack_sequence, pathlib, logging_silent
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240313-3.13.0a5+-8c094c3-PYTHON_UOPS/bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 0.94x