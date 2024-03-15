
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: fcdc84c
- commit date: 2024-01-29
- overall geometric mean: 1.00x slower
- HPT reliability: 96.94%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 284 ms: 1.07x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.49 ms: 1.12x slower                                                            |
| docutils       | 2.66 sec                                               | 2.73 sec: 1.02x slower                                                           |
| tornado_http   | 98.1 ms                                                | 99.2 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 450 ms: 1.17x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 576 ms: 1.11x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 461 ms: 1.07x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 723 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 740 ms: 1.03x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 611 ms: 1.03x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| float          | 78.9 ms                                                | 93.3 ms: 1.18x slower                                                            |
| nbody          | 96.0 ms                                                | 117 ms: 1.22x slower                                                             |
| Geometric mean | (ref)                                                  | 1.12x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.58 ms: 1.02x slower                                                            |
| regex_compile  | 141 ms                                                 | 152 ms: 1.08x slower                                                             |
| regex_dna      | 205 ms                                                 | 223 ms: 1.09x slower                                                             |
| regex_v8       | 22.9 ms                                                | 25.1 ms: 1.10x slower                                                            |
| Geometric mean | (ref)                                                  | 1.07x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 300 us: 1.06x faster                                                             |
| unpickle_list        | 5.21 us                                                | 5.05 us: 1.03x faster                                                            |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                                             |
| json_loads           | 29.2 us                                                | 28.3 us: 1.03x faster                                                            |
| unpickle_pure_python | 242 us                                                 | 236 us: 1.02x faster                                                             |
| pickle_dict          | 34.6 us                                                | 33.9 us: 1.02x faster                                                            |
| xml_etree_iterparse  | 108 ms                                                 | 112 ms: 1.03x slower                                                             |
| tomli_loads          | 2.30 sec                                               | 2.41 sec: 1.05x slower                                                           |
| pickle               | 11.0 us                                                | 11.8 us: 1.07x slower                                                            |
| xml_etree_process    | 56.9 ms                                                | 61.6 ms: 1.08x slower                                                            |
| pickle_list          | 4.59 us                                                | 5.01 us: 1.09x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 89.9 ms: 1.11x slower                                                            |
| unpickle             | 13.8 us                                                | 15.4 us: 1.11x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.78 ms: 1.46x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 14.1 ms: 1.33x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 118 us: 4.40x faster                                                             |
| generators                 | 74.9 ms                                                | 30.0 ms: 2.49x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 495 ms: 1.77x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.81 sec: 1.72x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                            |
| coroutines                 | 27.0 ms                                                | 22.3 ms: 1.21x faster                                                            |
| async_tree_none            | 528 ms                                                 | 450 ms: 1.17x faster                                                             |
| richards_super             | 61.9 ms                                                | 55.2 ms: 1.12x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 576 ms: 1.11x faster                                                             |
| comprehensions             | 23.6 us                                                | 21.8 us: 1.08x faster                                                            |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.08x faster                                                            |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 461 ms: 1.07x faster                                                             |
| pickle_pure_python         | 320 us                                                 | 300 us: 1.06x faster                                                             |
| mdp                        | 2.77 sec                                               | 2.63 sec: 1.06x faster                                                           |
| sqlglot_transpile          | 1.75 ms                                                | 1.66 ms: 1.05x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 161 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 723 ms: 1.04x faster                                                             |
| unpickle_list              | 5.21 us                                                | 5.05 us: 1.03x faster                                                            |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                                             |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| json_loads                 | 29.2 us                                                | 28.3 us: 1.03x faster                                                            |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 740 ms: 1.03x faster                                                             |
| raytrace                   | 309 ms                                                 | 300 ms: 1.03x faster                                                             |
| gc_traversal               | 4.01 ms                                                | 3.91 ms: 1.03x faster                                                            |
| async_tree_memoization_tg  | 626 ms                                                 | 611 ms: 1.03x faster                                                             |
| logging_silent             | 111 ns                                                 | 108 ns: 1.03x faster                                                             |
| deepcopy_reduce            | 3.22 us                                                | 3.14 us: 1.02x faster                                                            |
| unpickle_pure_python       | 242 us                                                 | 236 us: 1.02x faster                                                             |
| deepcopy                   | 365 us                                                 | 357 us: 1.02x faster                                                             |
| logging_simple             | 6.22 us                                                | 6.09 us: 1.02x faster                                                            |
| sympy_str                  | 297 ms                                                 | 291 ms: 1.02x faster                                                             |
| pickle_dict                | 34.6 us                                                | 33.9 us: 1.02x faster                                                            |
| richards                   | 49.8 ms                                                | 48.9 ms: 1.02x faster                                                            |
| json                       | 5.24 ms                                                | 5.15 ms: 1.02x faster                                                            |
| sympy_integrate            | 21.5 ms                                                | 21.1 ms: 1.02x faster                                                            |
| sympy_expand               | 484 ms                                                 | 487 ms: 1.01x slower                                                             |
| asyncio_websockets         | 550 ms                                                 | 554 ms: 1.01x slower                                                             |
| scimark_lu                 | 116 ms                                                 | 117 ms: 1.01x slower                                                             |
| dask                       | 365 ms                                                 | 369 ms: 1.01x slower                                                             |
| tornado_http               | 98.1 ms                                                | 99.2 ms: 1.01x slower                                                            |
| sqlglot_normalize          | 113 ms                                                 | 114 ms: 1.01x slower                                                             |
| bench_thread_pool          | 834 us                                                 | 848 us: 1.02x slower                                                             |
| pycparser                  | 1.19 sec                                               | 1.21 sec: 1.02x slower                                                           |
| deepcopy_memo              | 40.2 us                                                | 41.0 us: 1.02x slower                                                            |
| regex_effbot               | 3.51 ms                                                | 3.58 ms: 1.02x slower                                                            |
| chaos                      | 71.9 ms                                                | 73.4 ms: 1.02x slower                                                            |
| docutils                   | 2.66 sec                                               | 2.73 sec: 1.02x slower                                                           |
| scimark_sor                | 121 ms                                                 | 125 ms: 1.03x slower                                                             |
| pathlib                    | 18.5 ms                                                | 19.1 ms: 1.03x slower                                                            |
| xml_etree_iterparse        | 108 ms                                                 | 112 ms: 1.03x slower                                                             |
| create_gc_cycles           | 1.43 ms                                                | 1.48 ms: 1.03x slower                                                            |
| tomli_loads                | 2.30 sec                                               | 2.41 sec: 1.05x slower                                                           |
| go                         | 149 ms                                                 | 156 ms: 1.05x slower                                                             |
| sqlglot_optimize           | 55.3 ms                                                | 58.2 ms: 1.05x slower                                                            |
| meteor_contest             | 109 ms                                                 | 116 ms: 1.06x slower                                                             |
| dulwich_log                | 64.6 ms                                                | 68.8 ms: 1.07x slower                                                            |
| nqueens                    | 87.9 ms                                                | 93.8 ms: 1.07x slower                                                            |
| pickle                     | 11.0 us                                                | 11.8 us: 1.07x slower                                                            |
| 2to3                       | 264 ms                                                 | 284 ms: 1.07x slower                                                             |
| regex_compile              | 141 ms                                                 | 152 ms: 1.08x slower                                                             |
| xml_etree_process          | 56.9 ms                                                | 61.6 ms: 1.08x slower                                                            |
| regex_dna                  | 205 ms                                                 | 223 ms: 1.09x slower                                                             |
| pickle_list                | 4.59 us                                                | 5.01 us: 1.09x slower                                                            |
| fannkuch                   | 405 ms                                                 | 444 ms: 1.10x slower                                                             |
| regex_v8                   | 22.9 ms                                                | 25.1 ms: 1.10x slower                                                            |
| pprint_pformat             | 1.55 sec                                               | 1.71 sec: 1.10x slower                                                           |
| pprint_safe_repr           | 747 ms                                                 | 823 ms: 1.10x slower                                                             |
| xml_etree_generate         | 81.1 ms                                                | 89.9 ms: 1.11x slower                                                            |
| unpickle                   | 13.8 us                                                | 15.4 us: 1.11x slower                                                            |
| crypto_pyaes               | 76.7 ms                                                | 85.6 ms: 1.12x slower                                                            |
| chameleon                  | 6.70 ms                                                | 7.49 ms: 1.12x slower                                                            |
| sqlite_synth               | 2.57 us                                                | 2.88 us: 1.12x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 80.1 ms: 1.13x slower                                                            |
| float                      | 78.9 ms                                                | 93.3 ms: 1.18x slower                                                            |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.97 ms: 1.19x slower                                                            |
| pyflate                    | 434 ms                                                 | 519 ms: 1.20x slower                                                             |
| deltablue                  | 3.92 ms                                                | 4.70 ms: 1.20x slower                                                            |
| coverage                   | 78.8 ms                                                | 95.1 ms: 1.21x slower                                                            |
| unpack_sequence            | 43.5 ns                                                | 53.0 ns: 1.22x slower                                                            |
| nbody                      | 96.0 ms                                                | 117 ms: 1.22x slower                                                             |
| scimark_fft                | 345 ms                                                 | 426 ms: 1.23x slower                                                             |
| hexiom                     | 6.89 ms                                                | 8.51 ms: 1.24x slower                                                            |
| async_generators           | 374 ms                                                 | 462 ms: 1.24x slower                                                             |
| mypy2                      | 686 ms                                                 | 866 ms: 1.26x slower                                                             |
| telco                      | 6.86 ms                                                | 8.79 ms: 1.28x slower                                                            |
| spectral_norm              | 108 ms                                                 | 140 ms: 1.29x slower                                                             |
| mako                       | 10.7 ms                                                | 14.1 ms: 1.33x slower                                                            |
| python_startup_no_site     | 6.01 ms                                                | 8.78 ms: 1.46x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (2): bench_mp_pool, logging_format
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 96.94% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x