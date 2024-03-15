
# Results vs. 3.11.0

- fork: python
- ref: 4ee6bdfbaa792a3aa93c
- machine: linux-x86_64
- commit hash: 4ee6bdf
- commit date: 2024-02-22
- overall geometric mean: 1.01x slower \*
- HPT reliability: 93.16%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.14x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 288 ms: 1.09x slower                                                   |
| chameleon      | 6.70 ms                                                | 6.74 ms: 1.01x slower                                                  |
| docutils       | 2.66 sec                                               | 2.75 sec: 1.03x slower                                                 |
| tornado_http   | 98.1 ms                                                | 97.3 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 437 ms: 1.21x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 565 ms: 1.13x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 449 ms: 1.09x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 579 ms: 1.08x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 709 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 724 ms: 1.05x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.10x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                   |
| nbody          | 96.0 ms                                                | 100 ms: 1.05x slower                                                   |
| float          | 78.9 ms                                                | 83.7 ms: 1.06x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.63 ms: 1.04x slower                                                  |
| regex_v8       | 22.9 ms                                                | 24.4 ms: 1.07x slower                                                  |
| regex_dna      | 205 ms                                                 | 226 ms: 1.10x slower                                                   |
| regex_compile  | 141 ms                                                 | 169 ms: 1.19x slower                                                   |
| Geometric mean | (ref)                                                  | 1.10x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 295 us: 1.09x faster                                                   |
| json_loads           | 29.2 us                                                | 27.4 us: 1.06x faster                                                  |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                                   |
| unpickle_list        | 5.21 us                                                | 5.08 us: 1.03x faster                                                  |
| pickle_dict          | 34.6 us                                                | 34.2 us: 1.01x faster                                                  |
| xml_etree_process    | 56.9 ms                                                | 59.2 ms: 1.04x slower                                                  |
| pickle               | 11.0 us                                                | 11.5 us: 1.04x slower                                                  |
| unpickle_pure_python | 242 us                                                 | 254 us: 1.05x slower                                                   |
| unpickle             | 13.8 us                                                | 14.8 us: 1.07x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 87.2 ms: 1.08x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.20 us: 1.13x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (2): tomli_loads, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 11.7 ms: 1.36x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 10.3 ms: 1.72x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.53x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 12.1 ms: 1.13x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240222-linux-x86_64-python-4ee6bdfbaa792a3aa93c-3.13.0a4+-4ee6bdf |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 111 us: 4.68x faster                                                   |
| generators                 | 74.9 ms                                                | 29.6 ms: 2.53x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 489 ms: 1.79x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                 |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.1 ms: 1.22x faster                                                  |
| comprehensions             | 23.6 us                                                | 19.4 us: 1.22x faster                                                  |
| async_tree_none            | 528 ms                                                 | 437 ms: 1.21x faster                                                   |
| logging_silent             | 111 ns                                                 | 97.3 ns: 1.14x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 565 ms: 1.13x faster                                                   |
| deltablue                  | 3.92 ms                                                | 3.53 ms: 1.11x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 449 ms: 1.09x faster                                                   |
| logging_simple             | 6.22 us                                                | 5.72 us: 1.09x faster                                                  |
| pickle_pure_python         | 320 us                                                 | 295 us: 1.09x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 579 ms: 1.08x faster                                                   |
| richards_super             | 61.9 ms                                                | 57.2 ms: 1.08x faster                                                  |
| logging_format             | 6.81 us                                                | 6.31 us: 1.08x faster                                                  |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                 |
| json_loads                 | 29.2 us                                                | 27.4 us: 1.06x faster                                                  |
| deepcopy_reduce            | 3.22 us                                                | 3.04 us: 1.06x faster                                                  |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 709 ms: 1.06x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.80 ms: 1.05x faster                                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.36 ms: 1.05x faster                                                  |
| json                       | 5.24 ms                                                | 4.97 ms: 1.05x faster                                                  |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 724 ms: 1.05x faster                                                   |
| deepcopy                   | 365 us                                                 | 348 us: 1.05x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.04x faster                                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.68 ms: 1.04x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 162 ms: 1.04x faster                                                   |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                   |
| chaos                      | 71.9 ms                                                | 69.4 ms: 1.04x faster                                                  |
| sqlglot_normalize          | 113 ms                                                 | 109 ms: 1.03x faster                                                   |
| unpickle_list              | 5.21 us                                                | 5.08 us: 1.03x faster                                                  |
| sympy_str                  | 297 ms                                                 | 291 ms: 1.02x faster                                                   |
| sympy_integrate            | 21.5 ms                                                | 21.2 ms: 1.01x faster                                                  |
| pickle_dict                | 34.6 us                                                | 34.2 us: 1.01x faster                                                  |
| tornado_http               | 98.1 ms                                                | 97.3 ms: 1.01x faster                                                  |
| pathlib                    | 18.5 ms                                                | 18.6 ms: 1.01x slower                                                  |
| chameleon                  | 6.70 ms                                                | 6.74 ms: 1.01x slower                                                  |
| crypto_pyaes               | 76.7 ms                                                | 77.7 ms: 1.01x slower                                                  |
| bench_thread_pool          | 834 us                                                 | 851 us: 1.02x slower                                                   |
| mdp                        | 2.77 sec                                               | 2.83 sec: 1.02x slower                                                 |
| raytrace                   | 309 ms                                                 | 316 ms: 1.02x slower                                                   |
| sympy_expand               | 484 ms                                                 | 497 ms: 1.03x slower                                                   |
| docutils                   | 2.66 sec                                               | 2.75 sec: 1.03x slower                                                 |
| regex_effbot               | 3.51 ms                                                | 3.63 ms: 1.04x slower                                                  |
| meteor_contest             | 109 ms                                                 | 113 ms: 1.04x slower                                                   |
| richards                   | 49.8 ms                                                | 51.6 ms: 1.04x slower                                                  |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.23 ms: 1.04x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 59.2 ms: 1.04x slower                                                  |
| pickle                     | 11.0 us                                                | 11.5 us: 1.04x slower                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 57.9 ms: 1.05x slower                                                  |
| nbody                      | 96.0 ms                                                | 100 ms: 1.05x slower                                                   |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.05x slower                                                  |
| unpickle_pure_python       | 242 us                                                 | 254 us: 1.05x slower                                                   |
| scimark_fft                | 345 ms                                                 | 363 ms: 1.05x slower                                                   |
| float                      | 78.9 ms                                                | 83.7 ms: 1.06x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 24.4 ms: 1.07x slower                                                  |
| pycparser                  | 1.19 sec                                               | 1.27 sec: 1.07x slower                                                 |
| unpickle                   | 13.8 us                                                | 14.8 us: 1.07x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 87.2 ms: 1.08x slower                                                  |
| nqueens                    | 87.9 ms                                                | 95.5 ms: 1.09x slower                                                  |
| 2to3                       | 264 ms                                                 | 288 ms: 1.09x slower                                                   |
| fannkuch                   | 405 ms                                                 | 442 ms: 1.09x slower                                                   |
| scimark_sor                | 121 ms                                                 | 133 ms: 1.09x slower                                                   |
| sqlite_synth               | 2.57 us                                                | 2.82 us: 1.10x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 71.2 ms: 1.10x slower                                                  |
| regex_dna                  | 205 ms                                                 | 226 ms: 1.10x slower                                                   |
| mako                       | 10.7 ms                                                | 12.1 ms: 1.13x slower                                                  |
| pickle_list                | 4.59 us                                                | 5.20 us: 1.13x slower                                                  |
| go                         | 149 ms                                                 | 171 ms: 1.15x slower                                                   |
| scimark_monte_carlo        | 70.7 ms                                                | 81.4 ms: 1.15x slower                                                  |
| scimark_lu                 | 116 ms                                                 | 135 ms: 1.16x slower                                                   |
| spectral_norm              | 108 ms                                                 | 126 ms: 1.17x slower                                                   |
| bench_mp_pool              | 24.0 ms                                                | 28.2 ms: 1.17x slower                                                  |
| pprint_safe_repr           | 747 ms                                                 | 889 ms: 1.19x slower                                                   |
| regex_compile              | 141 ms                                                 | 169 ms: 1.19x slower                                                   |
| coverage                   | 78.8 ms                                                | 95.8 ms: 1.22x slower                                                  |
| telco                      | 6.86 ms                                                | 8.46 ms: 1.23x slower                                                  |
| pprint_pformat             | 1.55 sec                                               | 1.92 sec: 1.23x slower                                                 |
| pyflate                    | 434 ms                                                 | 543 ms: 1.25x slower                                                   |
| async_generators           | 374 ms                                                 | 470 ms: 1.26x slower                                                   |
| hexiom                     | 6.89 ms                                                | 8.80 ms: 1.28x slower                                                  |
| mypy2                      | 686 ms                                                 | 895 ms: 1.30x slower                                                   |
| python_startup             | 8.56 ms                                                | 11.7 ms: 1.36x slower                                                  |
| python_startup_no_site     | 6.01 ms                                                | 10.3 ms: 1.72x slower                                                  |
| unpack_sequence            | 43.5 ns                                                | 159 ns: 3.67x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (4): deepcopy_memo, tomli_loads, asyncio_websockets, xml_etree_iterparse
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 93.16% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.14x