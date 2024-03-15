
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.02x slower
- HPT reliability: 99.50%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 289 ms: 1.09x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.52 ms: 1.12x slower                                                            |
| docutils       | 2.66 sec                                               | 2.74 sec: 1.03x slower                                                           |
| tornado_http   | 98.1 ms                                                | 101 ms: 1.04x slower                                                             |
| Geometric mean | (ref)                                                  | 1.07x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 450 ms: 1.17x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 581 ms: 1.10x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 462 ms: 1.06x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 721 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 734 ms: 1.04x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 609 ms: 1.03x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                             |
| float          | 78.9 ms                                                | 101 ms: 1.28x slower                                                             |
| nbody          | 96.0 ms                                                | 135 ms: 1.41x slower                                                             |
| Geometric mean | (ref)                                                  | 1.21x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.54 ms: 1.01x slower                                                            |
| regex_v8       | 22.9 ms                                                | 24.5 ms: 1.07x slower                                                            |
| regex_dna      | 205 ms                                                 | 220 ms: 1.07x slower                                                             |
| regex_compile  | 141 ms                                                 | 156 ms: 1.11x slower                                                             |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 300 us: 1.07x faster                                                             |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                             |
| json_loads           | 29.2 us                                                | 28.2 us: 1.03x faster                                                            |
| unpickle_list        | 5.21 us                                                | 5.06 us: 1.03x faster                                                            |
| pickle_dict          | 34.6 us                                                | 34.2 us: 1.01x faster                                                            |
| unpickle_pure_python | 242 us                                                 | 240 us: 1.01x faster                                                             |
| pickle               | 11.0 us                                                | 11.6 us: 1.06x slower                                                            |
| xml_etree_iterparse  | 108 ms                                                 | 115 ms: 1.06x slower                                                             |
| xml_etree_process    | 56.9 ms                                                | 61.5 ms: 1.08x slower                                                            |
| unpickle             | 13.8 us                                                | 15.1 us: 1.09x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 90.0 ms: 1.11x slower                                                            |
| pickle_list          | 4.59 us                                                | 5.15 us: 1.12x slower                                                            |
| tomli_loads          | 2.30 sec                                               | 2.74 sec: 1.19x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.82 ms: 1.47x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 14.8 ms: 1.39x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 121 us: 4.30x faster                                                             |
| generators                 | 74.9 ms                                                | 29.9 ms: 2.50x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 500 ms: 1.75x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.81 sec: 1.72x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                            |
| coroutines                 | 27.0 ms                                                | 22.9 ms: 1.18x faster                                                            |
| async_tree_none            | 528 ms                                                 | 450 ms: 1.17x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 581 ms: 1.10x faster                                                             |
| gc_traversal               | 4.01 ms                                                | 3.65 ms: 1.10x faster                                                            |
| richards_super             | 61.9 ms                                                | 57.0 ms: 1.09x faster                                                            |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                           |
| pickle_pure_python         | 320 us                                                 | 300 us: 1.07x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 462 ms: 1.06x faster                                                             |
| sqlglot_parse              | 1.43 ms                                                | 1.35 ms: 1.06x faster                                                            |
| logging_silent             | 111 ns                                                 | 106 ns: 1.05x faster                                                             |
| mdp                        | 2.77 sec                                               | 2.66 sec: 1.04x faster                                                           |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 721 ms: 1.04x faster                                                             |
| sqlglot_transpile          | 1.75 ms                                                | 1.69 ms: 1.04x faster                                                            |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 734 ms: 1.04x faster                                                             |
| json_loads                 | 29.2 us                                                | 28.2 us: 1.03x faster                                                            |
| unpickle_list              | 5.21 us                                                | 5.06 us: 1.03x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 164 ms: 1.03x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 609 ms: 1.03x faster                                                             |
| deepcopy_reduce            | 3.22 us                                                | 3.13 us: 1.03x faster                                                            |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                             |
| logging_simple             | 6.22 us                                                | 6.08 us: 1.02x faster                                                            |
| deepcopy                   | 365 us                                                 | 357 us: 1.02x faster                                                             |
| comprehensions             | 23.6 us                                                | 23.1 us: 1.02x faster                                                            |
| json                       | 5.24 ms                                                | 5.18 ms: 1.01x faster                                                            |
| pickle_dict                | 34.6 us                                                | 34.2 us: 1.01x faster                                                            |
| pathlib                    | 18.5 ms                                                | 18.4 ms: 1.01x faster                                                            |
| unpickle_pure_python       | 242 us                                                 | 240 us: 1.01x faster                                                             |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                             |
| sympy_integrate            | 21.5 ms                                                | 21.6 ms: 1.01x slower                                                            |
| logging_format             | 6.81 us                                                | 6.87 us: 1.01x slower                                                            |
| regex_effbot               | 3.51 ms                                                | 3.54 ms: 1.01x slower                                                            |
| dask                       | 365 ms                                                 | 369 ms: 1.01x slower                                                             |
| raytrace                   | 309 ms                                                 | 312 ms: 1.01x slower                                                             |
| richards                   | 49.8 ms                                                | 50.6 ms: 1.02x slower                                                            |
| sympy_str                  | 297 ms                                                 | 303 ms: 1.02x slower                                                             |
| deepcopy_memo              | 40.2 us                                                | 41.0 us: 1.02x slower                                                            |
| bench_thread_pool          | 834 us                                                 | 855 us: 1.02x slower                                                             |
| create_gc_cycles           | 1.43 ms                                                | 1.47 ms: 1.03x slower                                                            |
| sqlglot_normalize          | 113 ms                                                 | 116 ms: 1.03x slower                                                             |
| docutils                   | 2.66 sec                                               | 2.74 sec: 1.03x slower                                                           |
| tornado_http               | 98.1 ms                                                | 101 ms: 1.04x slower                                                             |
| scimark_lu                 | 116 ms                                                 | 121 ms: 1.04x slower                                                             |
| sympy_expand               | 484 ms                                                 | 504 ms: 1.04x slower                                                             |
| pycparser                  | 1.19 sec                                               | 1.25 sec: 1.06x slower                                                           |
| pickle                     | 11.0 us                                                | 11.6 us: 1.06x slower                                                            |
| xml_etree_iterparse        | 108 ms                                                 | 115 ms: 1.06x slower                                                             |
| sqlglot_optimize           | 55.3 ms                                                | 59.0 ms: 1.07x slower                                                            |
| chaos                      | 71.9 ms                                                | 76.8 ms: 1.07x slower                                                            |
| dulwich_log                | 64.6 ms                                                | 69.2 ms: 1.07x slower                                                            |
| regex_v8                   | 22.9 ms                                                | 24.5 ms: 1.07x slower                                                            |
| scimark_sor                | 121 ms                                                 | 130 ms: 1.07x slower                                                             |
| regex_dna                  | 205 ms                                                 | 220 ms: 1.07x slower                                                             |
| go                         | 149 ms                                                 | 160 ms: 1.08x slower                                                             |
| xml_etree_process          | 56.9 ms                                                | 61.5 ms: 1.08x slower                                                            |
| meteor_contest             | 109 ms                                                 | 118 ms: 1.08x slower                                                             |
| 2to3                       | 264 ms                                                 | 289 ms: 1.09x slower                                                             |
| unpickle                   | 13.8 us                                                | 15.1 us: 1.09x slower                                                            |
| unpack_sequence            | 43.5 ns                                                | 47.8 ns: 1.10x slower                                                            |
| regex_compile              | 141 ms                                                 | 156 ms: 1.11x slower                                                             |
| xml_etree_generate         | 81.1 ms                                                | 90.0 ms: 1.11x slower                                                            |
| nqueens                    | 87.9 ms                                                | 98.6 ms: 1.12x slower                                                            |
| chameleon                  | 6.70 ms                                                | 7.52 ms: 1.12x slower                                                            |
| pickle_list                | 4.59 us                                                | 5.15 us: 1.12x slower                                                            |
| pprint_pformat             | 1.55 sec                                               | 1.75 sec: 1.13x slower                                                           |
| pprint_safe_repr           | 747 ms                                                 | 842 ms: 1.13x slower                                                             |
| sqlite_synth               | 2.57 us                                                | 2.92 us: 1.14x slower                                                            |
| fannkuch                   | 405 ms                                                 | 468 ms: 1.15x slower                                                             |
| crypto_pyaes               | 76.7 ms                                                | 90.4 ms: 1.18x slower                                                            |
| tomli_loads                | 2.30 sec                                               | 2.74 sec: 1.19x slower                                                           |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.06 ms: 1.21x slower                                                            |
| coverage                   | 78.8 ms                                                | 95.1 ms: 1.21x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 86.3 ms: 1.22x slower                                                            |
| async_generators           | 374 ms                                                 | 460 ms: 1.23x slower                                                             |
| pyflate                    | 434 ms                                                 | 540 ms: 1.25x slower                                                             |
| telco                      | 6.86 ms                                                | 8.66 ms: 1.26x slower                                                            |
| mypy2                      | 686 ms                                                 | 874 ms: 1.27x slower                                                             |
| float                      | 78.9 ms                                                | 101 ms: 1.28x slower                                                             |
| deltablue                  | 3.92 ms                                                | 5.18 ms: 1.32x slower                                                            |
| scimark_fft                | 345 ms                                                 | 459 ms: 1.33x slower                                                             |
| hexiom                     | 6.89 ms                                                | 9.23 ms: 1.34x slower                                                            |
| spectral_norm              | 108 ms                                                 | 145 ms: 1.34x slower                                                             |
| mako                       | 10.7 ms                                                | 14.8 ms: 1.39x slower                                                            |
| nbody                      | 96.0 ms                                                | 135 ms: 1.41x slower                                                             |
| python_startup_no_site     | 6.01 ms                                                | 8.82 ms: 1.47x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.50% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x