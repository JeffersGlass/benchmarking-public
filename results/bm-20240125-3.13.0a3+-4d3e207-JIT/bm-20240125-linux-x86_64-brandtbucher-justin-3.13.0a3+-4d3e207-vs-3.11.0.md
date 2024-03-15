
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: 4d3e207
- commit date: 2024-01-25
- overall geometric mean: 1.03x faster
- HPT reliability: 68.88%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 276 ms: 1.04x slower                                           |
| chameleon      | 6.70 ms                                                | 6.96 ms: 1.04x slower                                          |
| tornado_http   | 98.1 ms                                                | 97.4 ms: 1.01x faster                                          |
| Geometric mean | (ref)                                                  | 1.02x slower                                                   |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 446 ms: 1.18x faster                                           |
| async_tree_memoization     | 639 ms                                                 | 572 ms: 1.12x faster                                           |
| async_tree_none_tg         | 491 ms                                                 | 453 ms: 1.08x faster                                           |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.07x faster                                         |
| async_tree_memoization_tg  | 626 ms                                                 | 589 ms: 1.06x faster                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 715 ms: 1.05x faster                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 728 ms: 1.05x faster                                           |
| Geometric mean             | (ref)                                                  | 1.09x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                           |
| nbody          | 96.0 ms                                                | 104 ms: 1.08x slower                                           |
| float          | 78.9 ms                                                | 87.1 ms: 1.10x slower                                          |
| Geometric mean | (ref)                                                  | 1.05x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.62 ms: 1.03x slower                                          |
| regex_dna      | 205 ms                                                 | 220 ms: 1.08x slower                                           |
| regex_v8       | 22.9 ms                                                | 25.5 ms: 1.11x slower                                          |
| Geometric mean | (ref)                                                  | 1.05x slower                                                   |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.3 ms: 1.29x faster                                          |
| pickle_pure_python   | 320 us                                                 | 293 us: 1.09x faster                                           |
| unpickle_pure_python | 242 us                                                 | 229 us: 1.05x faster                                           |
| tomli_loads          | 2.30 sec                                               | 2.20 sec: 1.05x faster                                         |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                           |
| json_loads           | 29.2 us                                                | 28.2 us: 1.04x faster                                          |
| pickle_dict          | 34.6 us                                                | 34.0 us: 1.02x faster                                          |
| xml_etree_iterparse  | 108 ms                                                 | 109 ms: 1.01x slower                                           |
| unpickle_list        | 5.21 us                                                | 5.35 us: 1.03x slower                                          |
| xml_etree_process    | 56.9 ms                                                | 59.4 ms: 1.04x slower                                          |
| pickle               | 11.0 us                                                | 11.7 us: 1.07x slower                                          |
| xml_etree_generate   | 81.1 ms                                                | 87.9 ms: 1.08x slower                                          |
| unpickle             | 13.8 us                                                | 15.5 us: 1.12x slower                                          |
| pickle_list          | 4.59 us                                                | 5.23 us: 1.14x slower                                          |
| Geometric mean       | (ref)                                                  | 1.00x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                          |
| python_startup_no_site | 6.01 ms                                                | 8.82 ms: 1.47x slower                                          |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 12.7 ms: 1.19x slower                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 111 us: 4.66x faster                                           |
| generators                 | 74.9 ms                                                | 29.2 ms: 2.56x faster                                          |
| asyncio_tcp                | 875 ms                                                 | 490 ms: 1.79x faster                                           |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.73x faster                                         |
| json_dumps                 | 13.3 ms                                                | 10.3 ms: 1.29x faster                                          |
| comprehensions             | 23.6 us                                                | 19.6 us: 1.21x faster                                          |
| coroutines                 | 27.0 ms                                                | 22.5 ms: 1.20x faster                                          |
| richards_super             | 61.9 ms                                                | 51.9 ms: 1.19x faster                                          |
| async_tree_none            | 528 ms                                                 | 446 ms: 1.18x faster                                           |
| async_tree_memoization     | 639 ms                                                 | 572 ms: 1.12x faster                                           |
| sqlglot_parse              | 1.43 ms                                                | 1.28 ms: 1.11x faster                                          |
| raytrace                   | 309 ms                                                 | 282 ms: 1.09x faster                                           |
| pickle_pure_python         | 320 us                                                 | 293 us: 1.09x faster                                           |
| async_tree_none_tg         | 491 ms                                                 | 453 ms: 1.08x faster                                           |
| sqlglot_transpile          | 1.75 ms                                                | 1.62 ms: 1.08x faster                                          |
| richards                   | 49.8 ms                                                | 46.0 ms: 1.08x faster                                          |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.07x faster                                         |
| logging_simple             | 6.22 us                                                | 5.81 us: 1.07x faster                                          |
| logging_format             | 6.81 us                                                | 6.37 us: 1.07x faster                                          |
| async_tree_memoization_tg  | 626 ms                                                 | 589 ms: 1.06x faster                                           |
| gc_traversal               | 4.01 ms                                                | 3.77 ms: 1.06x faster                                          |
| unpickle_pure_python       | 242 us                                                 | 229 us: 1.05x faster                                           |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.05x faster                                           |
| mdp                        | 2.77 sec                                               | 2.64 sec: 1.05x faster                                         |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 715 ms: 1.05x faster                                           |
| tomli_loads                | 2.30 sec                                               | 2.20 sec: 1.05x faster                                         |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 728 ms: 1.05x faster                                           |
| deepcopy                   | 365 us                                                 | 350 us: 1.04x faster                                           |
| logging_silent             | 111 ns                                                 | 106 ns: 1.04x faster                                           |
| sympy_str                  | 297 ms                                                 | 285 ms: 1.04x faster                                           |
| deepcopy_reduce            | 3.22 us                                                | 3.09 us: 1.04x faster                                          |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                           |
| json_loads                 | 29.2 us                                                | 28.2 us: 1.04x faster                                          |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                           |
| sympy_integrate            | 21.5 ms                                                | 20.9 ms: 1.03x faster                                          |
| sqlglot_normalize          | 113 ms                                                 | 110 ms: 1.03x faster                                           |
| json                       | 5.24 ms                                                | 5.11 ms: 1.03x faster                                          |
| deepcopy_memo              | 40.2 us                                                | 39.2 us: 1.02x faster                                          |
| scimark_lu                 | 116 ms                                                 | 114 ms: 1.02x faster                                           |
| pathlib                    | 18.5 ms                                                | 18.2 ms: 1.02x faster                                          |
| pickle_dict                | 34.6 us                                                | 34.0 us: 1.02x faster                                          |
| chaos                      | 71.9 ms                                                | 70.8 ms: 1.01x faster                                          |
| sympy_expand               | 484 ms                                                 | 479 ms: 1.01x faster                                           |
| tornado_http               | 98.1 ms                                                | 97.4 ms: 1.01x faster                                          |
| bench_thread_pool          | 834 us                                                 | 837 us: 1.00x slower                                           |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                           |
| xml_etree_iterparse        | 108 ms                                                 | 109 ms: 1.01x slower                                           |
| scimark_sor                | 121 ms                                                 | 123 ms: 1.01x slower                                           |
| pycparser                  | 1.19 sec                                               | 1.20 sec: 1.01x slower                                         |
| meteor_contest             | 109 ms                                                 | 111 ms: 1.02x slower                                           |
| sqlglot_optimize           | 55.3 ms                                                | 56.5 ms: 1.02x slower                                          |
| nqueens                    | 87.9 ms                                                | 89.9 ms: 1.02x slower                                          |
| unpickle_list              | 5.21 us                                                | 5.35 us: 1.03x slower                                          |
| deltablue                  | 3.92 ms                                                | 4.05 ms: 1.03x slower                                          |
| regex_effbot               | 3.51 ms                                                | 3.62 ms: 1.03x slower                                          |
| crypto_pyaes               | 76.7 ms                                                | 79.3 ms: 1.03x slower                                          |
| chameleon                  | 6.70 ms                                                | 6.96 ms: 1.04x slower                                          |
| xml_etree_process          | 56.9 ms                                                | 59.4 ms: 1.04x slower                                          |
| 2to3                       | 264 ms                                                 | 276 ms: 1.04x slower                                           |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.05x slower                                          |
| dulwich_log                | 64.6 ms                                                | 67.9 ms: 1.05x slower                                          |
| scimark_monte_carlo        | 70.7 ms                                                | 74.6 ms: 1.06x slower                                          |
| pickle                     | 11.0 us                                                | 11.7 us: 1.07x slower                                          |
| fannkuch                   | 405 ms                                                 | 433 ms: 1.07x slower                                           |
| regex_dna                  | 205 ms                                                 | 220 ms: 1.08x slower                                           |
| nbody                      | 96.0 ms                                                | 104 ms: 1.08x slower                                           |
| xml_etree_generate         | 81.1 ms                                                | 87.9 ms: 1.08x slower                                          |
| pprint_pformat             | 1.55 sec                                               | 1.70 sec: 1.09x slower                                         |
| sqlite_synth               | 2.57 us                                                | 2.84 us: 1.10x slower                                          |
| float                      | 78.9 ms                                                | 87.1 ms: 1.10x slower                                          |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.55 ms: 1.10x slower                                          |
| pprint_safe_repr           | 747 ms                                                 | 827 ms: 1.11x slower                                           |
| scimark_fft                | 345 ms                                                 | 382 ms: 1.11x slower                                           |
| regex_v8                   | 22.9 ms                                                | 25.5 ms: 1.11x slower                                          |
| unpickle                   | 13.8 us                                                | 15.5 us: 1.12x slower                                          |
| pickle_list                | 4.59 us                                                | 5.23 us: 1.14x slower                                          |
| unpack_sequence            | 43.5 ns                                                | 49.7 ns: 1.14x slower                                          |
| hexiom                     | 6.89 ms                                                | 7.98 ms: 1.16x slower                                          |
| pyflate                    | 434 ms                                                 | 513 ms: 1.18x slower                                           |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                          |
| mako                       | 10.7 ms                                                | 12.7 ms: 1.19x slower                                          |
| coverage                   | 78.8 ms                                                | 94.1 ms: 1.19x slower                                          |
| async_generators           | 374 ms                                                 | 452 ms: 1.21x slower                                           |
| telco                      | 6.86 ms                                                | 8.54 ms: 1.25x slower                                          |
| mypy2                      | 686 ms                                                 | 864 ms: 1.26x slower                                           |
| spectral_norm              | 108 ms                                                 | 141 ms: 1.31x slower                                           |
| python_startup_no_site     | 6.01 ms                                                | 8.82 ms: 1.47x slower                                          |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                   |

Benchmark hidden because not significant (5): regex_compile, docutils, bench_mp_pool, dask, go
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 68.88% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x