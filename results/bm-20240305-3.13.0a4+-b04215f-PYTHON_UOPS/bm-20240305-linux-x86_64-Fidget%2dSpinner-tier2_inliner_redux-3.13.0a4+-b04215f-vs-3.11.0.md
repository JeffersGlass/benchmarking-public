# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_inliner_redux
- machine: linux-x86_64
- commit hash: b04215f
- commit date: 2024-03-05
- overall geometric mean: 1.07x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 300 ms: 1.13x slower                                                            |
| chameleon      | 6.70 ms                                                | 7.00 ms: 1.04x slower                                                           |
| docutils       | 2.66 sec                                               | 2.84 sec: 1.07x slower                                                          |
| tornado_http   | 98.1 ms                                                | 102 ms: 1.04x slower                                                            |
| Geometric mean | (ref)                                                  | 1.07x slower                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 462 ms: 1.14x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 592 ms: 1.08x faster                                                            |
| async_tree_memoization_tg  | 626 ms                                                 | 589 ms: 1.06x faster                                                            |
| async_tree_none_tg         | 491 ms                                                 | 462 ms: 1.06x faster                                                            |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 734 ms: 1.04x faster                                                            |
| async_tree_io_tg           | 1.29 sec                                               | 1.25 sec: 1.04x faster                                                          |
| async_tree_io              | 1.29 sec                                               | 1.25 sec: 1.03x faster                                                          |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 737 ms: 1.02x faster                                                            |
| Geometric mean             | (ref)                                                  | 1.06x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 190 ms: 1.02x faster                                                            |
| float          | 78.9 ms                                                | 106 ms: 1.34x slower                                                            |
| nbody          | 96.0 ms                                                | 132 ms: 1.38x slower                                                            |
| Geometric mean | (ref)                                                  | 1.22x slower                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.55 ms: 1.01x slower                                                           |
| regex_dna      | 205 ms                                                 | 213 ms: 1.04x slower                                                            |
| regex_v8       | 22.9 ms                                                | 24.4 ms: 1.07x slower                                                           |
| regex_compile  | 141 ms                                                 | 191 ms: 1.35x slower                                                            |
| Geometric mean | (ref)                                                  | 1.11x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.29x faster                                                           |
| pickle_pure_python   | 320 us                                                 | 303 us: 1.06x faster                                                            |
| json_loads           | 29.2 us                                                | 27.9 us: 1.05x faster                                                           |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                                            |
| unpickle_list        | 5.21 us                                                | 5.12 us: 1.02x faster                                                           |
| pickle_dict          | 34.6 us                                                | 35.1 us: 1.01x slower                                                           |
| xml_etree_iterparse  | 108 ms                                                 | 116 ms: 1.07x slower                                                            |
| pickle               | 11.0 us                                                | 11.9 us: 1.08x slower                                                           |
| xml_etree_process    | 56.9 ms                                                | 63.1 ms: 1.11x slower                                                           |
| unpickle             | 13.8 us                                                | 15.7 us: 1.13x slower                                                           |
| xml_etree_generate   | 81.1 ms                                                | 93.3 ms: 1.15x slower                                                           |
| pickle_list          | 4.59 us                                                | 5.33 us: 1.16x slower                                                           |
| tomli_loads          | 2.30 sec                                               | 2.79 sec: 1.21x slower                                                          |
| unpickle_pure_python | 242 us                                                 | 309 us: 1.28x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.05x slower                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.20x slower                                                           |
| python_startup_no_site | 6.01 ms                                                | 8.84 ms: 1.47x slower                                                           |
| Geometric mean         | (ref)                                                  | 1.33x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|-----------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 15.1 ms: 1.42x slower                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 119 us: 4.37x faster                                                            |
| generators                 | 74.9 ms                                                | 29.9 ms: 2.50x faster                                                           |
| asyncio_tcp                | 875 ms                                                 | 489 ms: 1.79x faster                                                            |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                          |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.29x faster                                                           |
| coroutines                 | 27.0 ms                                                | 22.7 ms: 1.19x faster                                                           |
| async_tree_none            | 528 ms                                                 | 462 ms: 1.14x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 592 ms: 1.08x faster                                                            |
| async_tree_memoization_tg  | 626 ms                                                 | 589 ms: 1.06x faster                                                            |
| async_tree_none_tg         | 491 ms                                                 | 462 ms: 1.06x faster                                                            |
| logging_silent             | 111 ns                                                 | 105 ns: 1.06x faster                                                            |
| pickle_pure_python         | 320 us                                                 | 303 us: 1.06x faster                                                            |
| json_loads                 | 29.2 us                                                | 27.9 us: 1.05x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 734 ms: 1.04x faster                                                            |
| logging_simple             | 6.22 us                                                | 6.00 us: 1.04x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.25 sec: 1.04x faster                                                          |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                                            |
| async_tree_io              | 1.29 sec                                               | 1.25 sec: 1.03x faster                                                          |
| pidigits                   | 194 ms                                                 | 190 ms: 1.02x faster                                                            |
| deepcopy_reduce            | 3.22 us                                                | 3.15 us: 1.02x faster                                                           |
| json                       | 5.24 ms                                                | 5.13 ms: 1.02x faster                                                           |
| unpickle_list              | 5.21 us                                                | 5.12 us: 1.02x faster                                                           |
| sympy_sum                  | 169 ms                                                 | 166 ms: 1.02x faster                                                            |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 737 ms: 1.02x faster                                                            |
| comprehensions             | 23.6 us                                                | 23.5 us: 1.00x faster                                                           |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                            |
| gc_traversal               | 4.01 ms                                                | 4.02 ms: 1.00x slower                                                           |
| sympy_integrate            | 21.5 ms                                                | 21.6 ms: 1.01x slower                                                           |
| sqlglot_normalize          | 113 ms                                                 | 114 ms: 1.01x slower                                                            |
| regex_effbot               | 3.51 ms                                                | 3.55 ms: 1.01x slower                                                           |
| pickle_dict                | 34.6 us                                                | 35.1 us: 1.01x slower                                                           |
| deltablue                  | 3.92 ms                                                | 4.02 ms: 1.03x slower                                                           |
| sympy_str                  | 297 ms                                                 | 306 ms: 1.03x slower                                                            |
| sqlglot_parse              | 1.43 ms                                                | 1.48 ms: 1.03x slower                                                           |
| pathlib                    | 18.5 ms                                                | 19.2 ms: 1.04x slower                                                           |
| mdp                        | 2.77 sec                                               | 2.88 sec: 1.04x slower                                                          |
| sqlglot_transpile          | 1.75 ms                                                | 1.82 ms: 1.04x slower                                                           |
| bench_thread_pool          | 834 us                                                 | 867 us: 1.04x slower                                                            |
| regex_dna                  | 205 ms                                                 | 213 ms: 1.04x slower                                                            |
| tornado_http               | 98.1 ms                                                | 102 ms: 1.04x slower                                                            |
| chameleon                  | 6.70 ms                                                | 7.00 ms: 1.04x slower                                                           |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.05x slower                                                           |
| sympy_expand               | 484 ms                                                 | 514 ms: 1.06x slower                                                            |
| regex_v8                   | 22.9 ms                                                | 24.4 ms: 1.07x slower                                                           |
| docutils                   | 2.66 sec                                               | 2.84 sec: 1.07x slower                                                          |
| xml_etree_iterparse        | 108 ms                                                 | 116 ms: 1.07x slower                                                            |
| pickle                     | 11.0 us                                                | 11.9 us: 1.08x slower                                                           |
| deepcopy_memo              | 40.2 us                                                | 43.8 us: 1.09x slower                                                           |
| richards_super             | 61.9 ms                                                | 67.7 ms: 1.09x slower                                                           |
| pycparser                  | 1.19 sec                                               | 1.30 sec: 1.10x slower                                                          |
| xml_etree_process          | 56.9 ms                                                | 63.1 ms: 1.11x slower                                                           |
| dulwich_log                | 64.6 ms                                                | 72.1 ms: 1.12x slower                                                           |
| chaos                      | 71.9 ms                                                | 80.3 ms: 1.12x slower                                                           |
| meteor_contest             | 109 ms                                                 | 122 ms: 1.12x slower                                                            |
| unpickle                   | 13.8 us                                                | 15.7 us: 1.13x slower                                                           |
| 2to3                       | 264 ms                                                 | 300 ms: 1.13x slower                                                            |
| sqlglot_optimize           | 55.3 ms                                                | 62.7 ms: 1.13x slower                                                           |
| xml_etree_generate         | 81.1 ms                                                | 93.3 ms: 1.15x slower                                                           |
| sqlite_synth               | 2.57 us                                                | 2.98 us: 1.16x slower                                                           |
| pickle_list                | 4.59 us                                                | 5.33 us: 1.16x slower                                                           |
| raytrace                   | 309 ms                                                 | 367 ms: 1.19x slower                                                            |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.20x slower                                                           |
| crypto_pyaes               | 76.7 ms                                                | 92.2 ms: 1.20x slower                                                           |
| tomli_loads                | 2.30 sec                                               | 2.79 sec: 1.21x slower                                                          |
| scimark_sor                | 121 ms                                                 | 148 ms: 1.22x slower                                                            |
| richards                   | 49.8 ms                                                | 61.2 ms: 1.23x slower                                                           |
| async_generators           | 374 ms                                                 | 462 ms: 1.24x slower                                                            |
| coverage                   | 78.8 ms                                                | 97.4 ms: 1.24x slower                                                           |
| pprint_pformat             | 1.55 sec                                               | 1.96 sec: 1.26x slower                                                          |
| pprint_safe_repr           | 747 ms                                                 | 945 ms: 1.26x slower                                                            |
| go                         | 149 ms                                                 | 190 ms: 1.28x slower                                                            |
| unpickle_pure_python       | 242 us                                                 | 309 us: 1.28x slower                                                            |
| nqueens                    | 87.9 ms                                                | 112 ms: 1.28x slower                                                            |
| telco                      | 6.86 ms                                                | 8.84 ms: 1.29x slower                                                           |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.53 ms: 1.30x slower                                                           |
| mypy2                      | 686 ms                                                 | 911 ms: 1.33x slower                                                            |
| fannkuch                   | 405 ms                                                 | 540 ms: 1.33x slower                                                            |
| float                      | 78.9 ms                                                | 106 ms: 1.34x slower                                                            |
| regex_compile              | 141 ms                                                 | 191 ms: 1.35x slower                                                            |
| scimark_fft                | 345 ms                                                 | 473 ms: 1.37x slower                                                            |
| nbody                      | 96.0 ms                                                | 132 ms: 1.38x slower                                                            |
| unpack_sequence            | 43.5 ns                                                | 61.2 ns: 1.41x slower                                                           |
| mako                       | 10.7 ms                                                | 15.1 ms: 1.42x slower                                                           |
| scimark_monte_carlo        | 70.7 ms                                                | 102 ms: 1.45x slower                                                            |
| scimark_lu                 | 116 ms                                                 | 169 ms: 1.46x slower                                                            |
| python_startup_no_site     | 6.01 ms                                                | 8.84 ms: 1.47x slower                                                           |
| dask                       | 365 ms                                                 | 538 ms: 1.47x slower                                                            |
| spectral_norm              | 108 ms                                                 | 162 ms: 1.50x slower                                                            |
| pyflate                    | 434 ms                                                 | 660 ms: 1.52x slower                                                            |
| hexiom                     | 6.89 ms                                                | 10.6 ms: 1.54x slower                                                           |
| Geometric mean             | (ref)                                                  | 1.07x slower                                                                    |

Benchmark hidden because not significant (3): logging_format, bench_mp_pool, deepcopy
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 1.00x