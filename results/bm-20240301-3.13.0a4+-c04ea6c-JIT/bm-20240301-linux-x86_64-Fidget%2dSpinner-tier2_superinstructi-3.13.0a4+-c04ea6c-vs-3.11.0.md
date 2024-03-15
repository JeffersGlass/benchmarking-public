# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_superinstructi
- machine: linux-x86_64
- commit hash: c04ea6c
- commit date: 2024-03-01
- overall geometric mean: 1.01x faster \*
- HPT reliability: 53.41%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.24x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 280 ms: 1.06x slower                                                             |
| chameleon      | 6.70 ms                                                | 6.99 ms: 1.04x slower                                                            |
| docutils       | 2.66 sec                                               | 2.74 sec: 1.03x slower                                                           |
| tornado_http   | 98.1 ms                                                | 96.3 ms: 1.02x faster                                                            |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 439 ms: 1.20x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 567 ms: 1.13x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 452 ms: 1.09x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 585 ms: 1.07x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 708 ms: 1.06x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 722 ms: 1.05x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.09x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                             |
| float          | 78.9 ms                                                | 82.7 ms: 1.05x slower                                                            |
| Geometric mean | (ref)                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.61 ms: 1.03x slower                                                            |
| regex_compile  | 141 ms                                                 | 153 ms: 1.08x slower                                                             |
| regex_v8       | 22.9 ms                                                | 25.2 ms: 1.10x slower                                                            |
| regex_dna      | 205 ms                                                 | 232 ms: 1.14x slower                                                             |
| Geometric mean | (ref)                                                  | 1.09x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.3 ms: 1.29x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 299 us: 1.07x faster                                                             |
| json_loads           | 29.2 us                                                | 27.3 us: 1.07x faster                                                            |
| tomli_loads          | 2.30 sec                                               | 2.16 sec: 1.06x faster                                                           |
| unpickle_list        | 5.21 us                                                | 4.93 us: 1.06x faster                                                            |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                                             |
| pickle_dict          | 34.6 us                                                | 34.1 us: 1.01x faster                                                            |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.01x faster                                                             |
| unpickle_pure_python | 242 us                                                 | 245 us: 1.01x slower                                                             |
| xml_etree_process    | 56.9 ms                                                | 58.7 ms: 1.03x slower                                                            |
| pickle               | 11.0 us                                                | 11.7 us: 1.06x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 86.8 ms: 1.07x slower                                                            |
| pickle_list          | 4.59 us                                                | 4.97 us: 1.08x slower                                                            |
| unpickle             | 13.8 us                                                | 16.2 us: 1.17x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 12.3 ms: 1.43x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 10.9 ms: 1.81x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.61x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.9 ms: 1.11x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.74x faster                                                             |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.56x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 492 ms: 1.78x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.72x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.3 ms: 1.29x faster                                                            |
| comprehensions             | 23.6 us                                                | 18.6 us: 1.27x faster                                                            |
| coroutines                 | 27.0 ms                                                | 22.1 ms: 1.22x faster                                                            |
| async_tree_none            | 528 ms                                                 | 439 ms: 1.20x faster                                                             |
| deltablue                  | 3.92 ms                                                | 3.46 ms: 1.13x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 567 ms: 1.13x faster                                                             |
| raytrace                   | 309 ms                                                 | 276 ms: 1.12x faster                                                             |
| chaos                      | 71.9 ms                                                | 64.8 ms: 1.11x faster                                                            |
| richards_super             | 61.9 ms                                                | 56.0 ms: 1.10x faster                                                            |
| logging_silent             | 111 ns                                                 | 101 ns: 1.10x faster                                                             |
| sqlglot_parse              | 1.43 ms                                                | 1.31 ms: 1.09x faster                                                            |
| async_tree_none_tg         | 491 ms                                                 | 452 ms: 1.09x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| gc_traversal               | 4.01 ms                                                | 3.72 ms: 1.08x faster                                                            |
| async_tree_memoization_tg  | 626 ms                                                 | 585 ms: 1.07x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| pickle_pure_python         | 320 us                                                 | 299 us: 1.07x faster                                                             |
| json_loads                 | 29.2 us                                                | 27.3 us: 1.07x faster                                                            |
| tomli_loads                | 2.30 sec                                               | 2.16 sec: 1.06x faster                                                           |
| sqlglot_transpile          | 1.75 ms                                                | 1.65 ms: 1.06x faster                                                            |
| logging_format             | 6.81 us                                                | 6.41 us: 1.06x faster                                                            |
| logging_simple             | 6.22 us                                                | 5.86 us: 1.06x faster                                                            |
| unpickle_list              | 5.21 us                                                | 4.93 us: 1.06x faster                                                            |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 708 ms: 1.06x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 722 ms: 1.05x faster                                                             |
| deepcopy                   | 365 us                                                 | 347 us: 1.05x faster                                                             |
| xml_etree_parse            | 164 ms                                                 | 156 ms: 1.05x faster                                                             |
| sympy_sum                  | 169 ms                                                 | 161 ms: 1.05x faster                                                             |
| mdp                        | 2.77 sec                                               | 2.66 sec: 1.04x faster                                                           |
| sympy_str                  | 297 ms                                                 | 286 ms: 1.04x faster                                                             |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                             |
| sqlglot_normalize          | 113 ms                                                 | 109 ms: 1.03x faster                                                             |
| deepcopy_reduce            | 3.22 us                                                | 3.12 us: 1.03x faster                                                            |
| deepcopy_memo              | 40.2 us                                                | 39.0 us: 1.03x faster                                                            |
| json                       | 5.24 ms                                                | 5.10 ms: 1.03x faster                                                            |
| crypto_pyaes               | 76.7 ms                                                | 74.7 ms: 1.03x faster                                                            |
| tornado_http               | 98.1 ms                                                | 96.3 ms: 1.02x faster                                                            |
| pickle_dict                | 34.6 us                                                | 34.1 us: 1.01x faster                                                            |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.01x faster                                                             |
| meteor_contest             | 109 ms                                                 | 108 ms: 1.00x faster                                                             |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                             |
| pathlib                    | 18.5 ms                                                | 18.6 ms: 1.00x slower                                                            |
| richards                   | 49.8 ms                                                | 50.1 ms: 1.01x slower                                                            |
| unpickle_pure_python       | 242 us                                                 | 245 us: 1.01x slower                                                             |
| bench_thread_pool          | 834 us                                                 | 849 us: 1.02x slower                                                             |
| pycparser                  | 1.19 sec                                               | 1.21 sec: 1.02x slower                                                           |
| scimark_fft                | 345 ms                                                 | 354 ms: 1.03x slower                                                             |
| sqlglot_optimize           | 55.3 ms                                                | 56.7 ms: 1.03x slower                                                            |
| docutils                   | 2.66 sec                                               | 2.74 sec: 1.03x slower                                                           |
| regex_effbot               | 3.51 ms                                                | 3.61 ms: 1.03x slower                                                            |
| xml_etree_process          | 56.9 ms                                                | 58.7 ms: 1.03x slower                                                            |
| fannkuch                   | 405 ms                                                 | 419 ms: 1.03x slower                                                             |
| nqueens                    | 87.9 ms                                                | 91.4 ms: 1.04x slower                                                            |
| chameleon                  | 6.70 ms                                                | 6.99 ms: 1.04x slower                                                            |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.05x slower                                                            |
| float                      | 78.9 ms                                                | 82.7 ms: 1.05x slower                                                            |
| go                         | 149 ms                                                 | 156 ms: 1.05x slower                                                             |
| 2to3                       | 264 ms                                                 | 280 ms: 1.06x slower                                                             |
| pickle                     | 11.0 us                                                | 11.7 us: 1.06x slower                                                            |
| xml_etree_generate         | 81.1 ms                                                | 86.8 ms: 1.07x slower                                                            |
| scimark_sor                | 121 ms                                                 | 130 ms: 1.07x slower                                                             |
| dulwich_log                | 64.6 ms                                                | 69.3 ms: 1.07x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 76.2 ms: 1.08x slower                                                            |
| regex_compile              | 141 ms                                                 | 153 ms: 1.08x slower                                                             |
| pickle_list                | 4.59 us                                                | 4.97 us: 1.08x slower                                                            |
| sqlite_synth               | 2.57 us                                                | 2.81 us: 1.09x slower                                                            |
| regex_v8                   | 22.9 ms                                                | 25.2 ms: 1.10x slower                                                            |
| pprint_pformat             | 1.55 sec                                               | 1.72 sec: 1.10x slower                                                           |
| spectral_norm              | 108 ms                                                 | 120 ms: 1.11x slower                                                             |
| pprint_safe_repr           | 747 ms                                                 | 831 ms: 1.11x slower                                                             |
| mako                       | 10.7 ms                                                | 11.9 ms: 1.11x slower                                                            |
| hexiom                     | 6.89 ms                                                | 7.74 ms: 1.12x slower                                                            |
| scimark_lu                 | 116 ms                                                 | 131 ms: 1.13x slower                                                             |
| regex_dna                  | 205 ms                                                 | 232 ms: 1.14x slower                                                             |
| bench_mp_pool              | 24.0 ms                                                | 28.0 ms: 1.17x slower                                                            |
| unpickle                   | 13.8 us                                                | 16.2 us: 1.17x slower                                                            |
| pyflate                    | 434 ms                                                 | 509 ms: 1.17x slower                                                             |
| coverage                   | 78.8 ms                                                | 96.3 ms: 1.22x slower                                                            |
| async_generators           | 374 ms                                                 | 463 ms: 1.24x slower                                                             |
| telco                      | 6.86 ms                                                | 8.59 ms: 1.25x slower                                                            |
| mypy2                      | 686 ms                                                 | 895 ms: 1.31x slower                                                             |
| python_startup             | 8.56 ms                                                | 12.3 ms: 1.43x slower                                                            |
| python_startup_no_site     | 6.01 ms                                                | 10.9 ms: 1.81x slower                                                            |
| unpack_sequence            | 43.5 ns                                                | 126 ns: 2.91x slower                                                             |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (4): sympy_expand, sympy_integrate, nbody, scimark_sparse_mat_mult
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 53.41% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.24x