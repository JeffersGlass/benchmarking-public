
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.01x faster
- HPT reliability: 92.49%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 283 ms: 1.07x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.16 ms: 1.07x slower                                                            |
| docutils       | 2.66 sec                                               | 2.69 sec: 1.01x slower                                                           |
| Geometric mean | (ref)                                                  | 1.04x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 448 ms: 1.18x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 573 ms: 1.11x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 456 ms: 1.08x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 590 ms: 1.06x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 717 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 733 ms: 1.04x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| float          | 78.9 ms                                                | 87.7 ms: 1.11x slower                                                            |
| nbody          | 96.0 ms                                                | 113 ms: 1.17x slower                                                             |
| Geometric mean | (ref)                                                  | 1.08x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.56 ms: 1.02x slower                                                            |
| regex_compile  | 141 ms                                                 | 148 ms: 1.05x slower                                                             |
| regex_dna      | 205 ms                                                 | 222 ms: 1.08x slower                                                             |
| regex_v8       | 22.9 ms                                                | 24.9 ms: 1.09x slower                                                            |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 297 us: 1.08x faster                                                             |
| unpickle_list        | 5.21 us                                                | 4.94 us: 1.06x faster                                                            |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                                             |
| unpickle_pure_python | 242 us                                                 | 234 us: 1.03x faster                                                             |
| json_loads           | 29.2 us                                                | 28.3 us: 1.03x faster                                                            |
| pickle_dict          | 34.6 us                                                | 34.8 us: 1.01x slower                                                            |
| xml_etree_iterparse  | 108 ms                                                 | 110 ms: 1.02x slower                                                             |
| pickle               | 11.0 us                                                | 11.6 us: 1.06x slower                                                            |
| xml_etree_process    | 56.9 ms                                                | 60.5 ms: 1.06x slower                                                            |
| unpickle             | 13.8 us                                                | 15.0 us: 1.08x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 89.1 ms: 1.10x slower                                                            |
| pickle_list          | 4.59 us                                                | 5.23 us: 1.14x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (1): tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.19x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.79 ms: 1.46x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 12.9 ms: 1.21x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 116 us: 4.48x faster                                                             |
| generators                 | 74.9 ms                                                | 29.8 ms: 2.52x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 488 ms: 1.80x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                            |
| coroutines                 | 27.0 ms                                                | 22.7 ms: 1.19x faster                                                            |
| async_tree_none            | 528 ms                                                 | 448 ms: 1.18x faster                                                             |
| comprehensions             | 23.6 us                                                | 20.6 us: 1.15x faster                                                            |
| richards_super             | 61.9 ms                                                | 55.3 ms: 1.12x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 573 ms: 1.11x faster                                                             |
| sqlglot_parse              | 1.43 ms                                                | 1.32 ms: 1.08x faster                                                            |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| gc_traversal               | 4.01 ms                                                | 3.72 ms: 1.08x faster                                                            |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 456 ms: 1.08x faster                                                             |
| pickle_pure_python         | 320 us                                                 | 297 us: 1.08x faster                                                             |
| logging_silent             | 111 ns                                                 | 104 ns: 1.07x faster                                                             |
| unpack_sequence            | 43.5 ns                                                | 40.7 ns: 1.07x faster                                                            |
| mdp                        | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                           |
| sympy_sum                  | 169 ms                                                 | 159 ms: 1.06x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 590 ms: 1.06x faster                                                             |
| sqlglot_transpile          | 1.75 ms                                                | 1.65 ms: 1.06x faster                                                            |
| unpickle_list              | 5.21 us                                                | 4.94 us: 1.06x faster                                                            |
| raytrace                   | 309 ms                                                 | 294 ms: 1.05x faster                                                             |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 717 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 733 ms: 1.04x faster                                                             |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| unpickle_pure_python       | 242 us                                                 | 234 us: 1.03x faster                                                             |
| json_loads                 | 29.2 us                                                | 28.3 us: 1.03x faster                                                            |
| logging_simple             | 6.22 us                                                | 6.06 us: 1.03x faster                                                            |
| sympy_str                  | 297 ms                                                 | 290 ms: 1.03x faster                                                             |
| chaos                      | 71.9 ms                                                | 70.2 ms: 1.02x faster                                                            |
| sympy_integrate            | 21.5 ms                                                | 21.1 ms: 1.02x faster                                                            |
| richards                   | 49.8 ms                                                | 48.9 ms: 1.02x faster                                                            |
| json                       | 5.24 ms                                                | 5.17 ms: 1.01x faster                                                            |
| deepcopy                   | 365 us                                                 | 361 us: 1.01x faster                                                             |
| deepcopy_reduce            | 3.22 us                                                | 3.19 us: 1.01x faster                                                            |
| logging_format             | 6.81 us                                                | 6.76 us: 1.01x faster                                                            |
| sqlglot_normalize          | 113 ms                                                 | 113 ms: 1.00x slower                                                             |
| asyncio_websockets         | 550 ms                                                 | 553 ms: 1.00x slower                                                             |
| pickle_dict                | 34.6 us                                                | 34.8 us: 1.01x slower                                                            |
| sympy_expand               | 484 ms                                                 | 487 ms: 1.01x slower                                                             |
| pathlib                    | 18.5 ms                                                | 18.6 ms: 1.01x slower                                                            |
| docutils                   | 2.66 sec                                               | 2.69 sec: 1.01x slower                                                           |
| bench_thread_pool          | 834 us                                                 | 842 us: 1.01x slower                                                             |
| pycparser                  | 1.19 sec                                               | 1.20 sec: 1.01x slower                                                           |
| xml_etree_iterparse        | 108 ms                                                 | 110 ms: 1.02x slower                                                             |
| regex_effbot               | 3.51 ms                                                | 3.56 ms: 1.02x slower                                                            |
| deepcopy_memo              | 40.2 us                                                | 40.9 us: 1.02x slower                                                            |
| scimark_lu                 | 116 ms                                                 | 120 ms: 1.03x slower                                                             |
| create_gc_cycles           | 1.43 ms                                                | 1.48 ms: 1.03x slower                                                            |
| sqlglot_optimize           | 55.3 ms                                                | 57.6 ms: 1.04x slower                                                            |
| go                         | 149 ms                                                 | 155 ms: 1.04x slower                                                             |
| meteor_contest             | 109 ms                                                 | 114 ms: 1.05x slower                                                             |
| nqueens                    | 87.9 ms                                                | 92.2 ms: 1.05x slower                                                            |
| regex_compile              | 141 ms                                                 | 148 ms: 1.05x slower                                                             |
| scimark_sor                | 121 ms                                                 | 128 ms: 1.05x slower                                                             |
| pickle                     | 11.0 us                                                | 11.6 us: 1.06x slower                                                            |
| fannkuch                   | 405 ms                                                 | 429 ms: 1.06x slower                                                             |
| xml_etree_process          | 56.9 ms                                                | 60.5 ms: 1.06x slower                                                            |
| dulwich_log                | 64.6 ms                                                | 68.8 ms: 1.07x slower                                                            |
| pprint_pformat             | 1.55 sec                                               | 1.66 sec: 1.07x slower                                                           |
| chameleon                  | 6.70 ms                                                | 7.16 ms: 1.07x slower                                                            |
| 2to3                       | 264 ms                                                 | 283 ms: 1.07x slower                                                             |
| crypto_pyaes               | 76.7 ms                                                | 82.2 ms: 1.07x slower                                                            |
| pprint_safe_repr           | 747 ms                                                 | 806 ms: 1.08x slower                                                             |
| unpickle                   | 13.8 us                                                | 15.0 us: 1.08x slower                                                            |
| regex_dna                  | 205 ms                                                 | 222 ms: 1.08x slower                                                             |
| regex_v8                   | 22.9 ms                                                | 24.9 ms: 1.09x slower                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.50 ms: 1.09x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 77.5 ms: 1.10x slower                                                            |
| xml_etree_generate         | 81.1 ms                                                | 89.1 ms: 1.10x slower                                                            |
| float                      | 78.9 ms                                                | 87.7 ms: 1.11x slower                                                            |
| sqlite_synth               | 2.57 us                                                | 2.88 us: 1.12x slower                                                            |
| deltablue                  | 3.92 ms                                                | 4.41 ms: 1.12x slower                                                            |
| pickle_list                | 4.59 us                                                | 5.23 us: 1.14x slower                                                            |
| hexiom                     | 6.89 ms                                                | 8.01 ms: 1.16x slower                                                            |
| pyflate                    | 434 ms                                                 | 508 ms: 1.17x slower                                                             |
| nbody                      | 96.0 ms                                                | 113 ms: 1.17x slower                                                             |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.19x slower                                                            |
| coverage                   | 78.8 ms                                                | 93.5 ms: 1.19x slower                                                            |
| scimark_fft                | 345 ms                                                 | 414 ms: 1.20x slower                                                             |
| mako                       | 10.7 ms                                                | 12.9 ms: 1.21x slower                                                            |
| async_generators           | 374 ms                                                 | 456 ms: 1.22x slower                                                             |
| spectral_norm              | 108 ms                                                 | 132 ms: 1.22x slower                                                             |
| telco                      | 6.86 ms                                                | 8.62 ms: 1.26x slower                                                            |
| mypy2                      | 686 ms                                                 | 864 ms: 1.26x slower                                                             |
| python_startup_no_site     | 6.01 ms                                                | 8.79 ms: 1.46x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (4): bench_mp_pool, tomli_loads, tornado_http, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 92.49% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x