
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 6e55480
- commit date: 2024-01-24
- overall geometric mean: 1.01x faster
- HPT reliability: 96.18%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 286 ms: 1.08x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.33 ms: 1.09x slower                                                            |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                           |
| tornado_http   | 98.1 ms                                                | 99.2 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 447 ms: 1.18x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 571 ms: 1.12x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 455 ms: 1.08x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 599 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 717 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 734 ms: 1.04x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| float          | 78.9 ms                                                | 87.8 ms: 1.11x slower                                                            |
| nbody          | 96.0 ms                                                | 110 ms: 1.14x slower                                                             |
| Geometric mean | (ref)                                                  | 1.07x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.64 ms: 1.04x slower                                                            |
| regex_compile  | 141 ms                                                 | 149 ms: 1.06x slower                                                             |
| regex_v8       | 22.9 ms                                                | 24.7 ms: 1.08x slower                                                            |
| regex_dna      | 205 ms                                                 | 223 ms: 1.09x slower                                                             |
| Geometric mean | (ref)                                                  | 1.07x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 300 us: 1.07x faster                                                             |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.05x faster                                                             |
| unpickle_pure_python | 242 us                                                 | 235 us: 1.03x faster                                                             |
| json_loads           | 29.2 us                                                | 28.8 us: 1.01x faster                                                            |
| pickle_dict          | 34.6 us                                                | 34.9 us: 1.01x slower                                                            |
| xml_etree_iterparse  | 108 ms                                                 | 110 ms: 1.02x slower                                                             |
| unpickle_list        | 5.21 us                                                | 5.31 us: 1.02x slower                                                            |
| pickle               | 11.0 us                                                | 11.5 us: 1.05x slower                                                            |
| xml_etree_process    | 56.9 ms                                                | 60.8 ms: 1.07x slower                                                            |
| tomli_loads          | 2.30 sec                                               | 2.47 sec: 1.07x slower                                                           |
| unpickle             | 13.8 us                                                | 14.9 us: 1.07x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 88.5 ms: 1.09x slower                                                            |
| pickle_list          | 4.59 us                                                | 5.24 us: 1.14x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.84 ms: 1.47x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.3 ms: 1.25x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 117 us: 4.45x faster                                                             |
| generators                 | 74.9 ms                                                | 29.6 ms: 2.53x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 469 ms: 1.87x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.74x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                            |
| coroutines                 | 27.0 ms                                                | 22.3 ms: 1.21x faster                                                            |
| async_tree_none            | 528 ms                                                 | 447 ms: 1.18x faster                                                             |
| comprehensions             | 23.6 us                                                | 20.5 us: 1.15x faster                                                            |
| richards_super             | 61.9 ms                                                | 54.5 ms: 1.13x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 571 ms: 1.12x faster                                                             |
| unpack_sequence            | 43.5 ns                                                | 39.0 ns: 1.11x faster                                                            |
| sqlglot_parse              | 1.43 ms                                                | 1.32 ms: 1.08x faster                                                            |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 455 ms: 1.08x faster                                                             |
| pickle_pure_python         | 320 us                                                 | 300 us: 1.07x faster                                                             |
| logging_silent             | 111 ns                                                 | 105 ns: 1.06x faster                                                             |
| sqlglot_transpile          | 1.75 ms                                                | 1.65 ms: 1.06x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.06x faster                                                             |
| gc_traversal               | 4.01 ms                                                | 3.82 ms: 1.05x faster                                                            |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.05x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 599 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 717 ms: 1.04x faster                                                             |
| raytrace                   | 309 ms                                                 | 297 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 734 ms: 1.04x faster                                                             |
| richards                   | 49.8 ms                                                | 48.2 ms: 1.03x faster                                                            |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| sympy_str                  | 297 ms                                                 | 288 ms: 1.03x faster                                                             |
| unpickle_pure_python       | 242 us                                                 | 235 us: 1.03x faster                                                             |
| sympy_integrate            | 21.5 ms                                                | 20.9 ms: 1.03x faster                                                            |
| logging_simple             | 6.22 us                                                | 6.06 us: 1.03x faster                                                            |
| chaos                      | 71.9 ms                                                | 70.5 ms: 1.02x faster                                                            |
| json_loads                 | 29.2 us                                                | 28.8 us: 1.01x faster                                                            |
| deepcopy                   | 365 us                                                 | 360 us: 1.01x faster                                                             |
| deepcopy_reduce            | 3.22 us                                                | 3.17 us: 1.01x faster                                                            |
| json                       | 5.24 ms                                                | 5.20 ms: 1.01x faster                                                            |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                             |
| mdp                        | 2.77 sec                                               | 2.79 sec: 1.00x slower                                                           |
| logging_format             | 6.81 us                                                | 6.86 us: 1.01x slower                                                            |
| bench_thread_pool          | 834 us                                                 | 842 us: 1.01x slower                                                             |
| pickle_dict                | 34.6 us                                                | 34.9 us: 1.01x slower                                                            |
| sqlglot_normalize          | 113 ms                                                 | 114 ms: 1.01x slower                                                             |
| tornado_http               | 98.1 ms                                                | 99.2 ms: 1.01x slower                                                            |
| deepcopy_memo              | 40.2 us                                                | 40.6 us: 1.01x slower                                                            |
| docutils                   | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                           |
| xml_etree_iterparse        | 108 ms                                                 | 110 ms: 1.02x slower                                                             |
| unpickle_list              | 5.21 us                                                | 5.31 us: 1.02x slower                                                            |
| pathlib                    | 18.5 ms                                                | 18.9 ms: 1.02x slower                                                            |
| create_gc_cycles           | 1.43 ms                                                | 1.47 ms: 1.02x slower                                                            |
| scimark_lu                 | 116 ms                                                 | 119 ms: 1.02x slower                                                             |
| nqueens                    | 87.9 ms                                                | 90.5 ms: 1.03x slower                                                            |
| scimark_sor                | 121 ms                                                 | 125 ms: 1.03x slower                                                             |
| go                         | 149 ms                                                 | 153 ms: 1.03x slower                                                             |
| regex_effbot               | 3.51 ms                                                | 3.64 ms: 1.04x slower                                                            |
| meteor_contest             | 109 ms                                                 | 114 ms: 1.04x slower                                                             |
| sqlglot_optimize           | 55.3 ms                                                | 57.8 ms: 1.05x slower                                                            |
| pickle                     | 11.0 us                                                | 11.5 us: 1.05x slower                                                            |
| pycparser                  | 1.19 sec                                               | 1.25 sec: 1.05x slower                                                           |
| regex_compile              | 141 ms                                                 | 149 ms: 1.06x slower                                                             |
| dulwich_log                | 64.6 ms                                                | 68.8 ms: 1.07x slower                                                            |
| xml_etree_process          | 56.9 ms                                                | 60.8 ms: 1.07x slower                                                            |
| tomli_loads                | 2.30 sec                                               | 2.47 sec: 1.07x slower                                                           |
| crypto_pyaes               | 76.7 ms                                                | 82.3 ms: 1.07x slower                                                            |
| pprint_pformat             | 1.55 sec                                               | 1.67 sec: 1.07x slower                                                           |
| unpickle                   | 13.8 us                                                | 14.9 us: 1.07x slower                                                            |
| fannkuch                   | 405 ms                                                 | 437 ms: 1.08x slower                                                             |
| 2to3                       | 264 ms                                                 | 286 ms: 1.08x slower                                                             |
| regex_v8                   | 22.9 ms                                                | 24.7 ms: 1.08x slower                                                            |
| pprint_safe_repr           | 747 ms                                                 | 811 ms: 1.08x slower                                                             |
| xml_etree_generate         | 81.1 ms                                                | 88.5 ms: 1.09x slower                                                            |
| regex_dna                  | 205 ms                                                 | 223 ms: 1.09x slower                                                             |
| chameleon                  | 6.70 ms                                                | 7.33 ms: 1.09x slower                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.57 ms: 1.11x slower                                                            |
| float                      | 78.9 ms                                                | 87.8 ms: 1.11x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 78.8 ms: 1.11x slower                                                            |
| sqlite_synth               | 2.57 us                                                | 2.87 us: 1.12x slower                                                            |
| deltablue                  | 3.92 ms                                                | 4.42 ms: 1.13x slower                                                            |
| pickle_list                | 4.59 us                                                | 5.24 us: 1.14x slower                                                            |
| nbody                      | 96.0 ms                                                | 110 ms: 1.14x slower                                                             |
| hexiom                     | 6.89 ms                                                | 7.97 ms: 1.16x slower                                                            |
| pyflate                    | 434 ms                                                 | 516 ms: 1.19x slower                                                             |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| coverage                   | 78.8 ms                                                | 95.4 ms: 1.21x slower                                                            |
| scimark_fft                | 345 ms                                                 | 419 ms: 1.21x slower                                                             |
| async_generators           | 374 ms                                                 | 456 ms: 1.22x slower                                                             |
| mako                       | 10.7 ms                                                | 13.3 ms: 1.25x slower                                                            |
| spectral_norm              | 108 ms                                                 | 136 ms: 1.26x slower                                                             |
| mypy2                      | 686 ms                                                 | 867 ms: 1.26x slower                                                             |
| telco                      | 6.86 ms                                                | 8.71 ms: 1.27x slower                                                            |
| python_startup_no_site     | 6.01 ms                                                | 8.84 ms: 1.47x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (3): bench_mp_pool, sympy_expand, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 96.18% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x