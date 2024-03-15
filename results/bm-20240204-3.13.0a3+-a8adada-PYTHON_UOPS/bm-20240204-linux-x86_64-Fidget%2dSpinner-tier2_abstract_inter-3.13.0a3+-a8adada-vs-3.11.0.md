
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: a8adada
- commit date: 2024-02-04
- overall geometric mean: 1.01x faster \*
- HPT reliability: 93.47%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 282 ms: 1.07x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.27 ms: 1.08x slower                                                            |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                           |
| Geometric mean | (ref)                                                  | 1.04x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 452 ms: 1.17x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 578 ms: 1.11x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 459 ms: 1.07x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.07x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 603 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 737 ms: 1.03x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 727 ms: 1.03x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| float          | 78.9 ms                                                | 92.0 ms: 1.17x slower                                                            |
| nbody          | 96.0 ms                                                | 119 ms: 1.24x slower                                                             |
| Geometric mean | (ref)                                                  | 1.12x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.66 ms: 1.04x slower                                                            |
| regex_compile  | 141 ms                                                 | 149 ms: 1.05x slower                                                             |
| regex_v8       | 22.9 ms                                                | 24.2 ms: 1.06x slower                                                            |
| regex_dna      | 205 ms                                                 | 221 ms: 1.08x slower                                                             |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.25x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 299 us: 1.07x faster                                                             |
| unpickle_list        | 5.21 us                                                | 4.96 us: 1.05x faster                                                            |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                             |
| unpickle_pure_python | 242 us                                                 | 234 us: 1.03x faster                                                             |
| json_loads           | 29.2 us                                                | 28.7 us: 1.02x faster                                                            |
| xml_etree_iterparse  | 108 ms                                                 | 109 ms: 1.01x slower                                                             |
| pickle_dict          | 34.6 us                                                | 35.1 us: 1.01x slower                                                            |
| tomli_loads          | 2.30 sec                                               | 2.35 sec: 1.02x slower                                                           |
| pickle               | 11.0 us                                                | 11.6 us: 1.05x slower                                                            |
| xml_etree_process    | 56.9 ms                                                | 60.4 ms: 1.06x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 88.9 ms: 1.10x slower                                                            |
| pickle_list          | 4.59 us                                                | 5.12 us: 1.12x slower                                                            |
| unpickle             | 13.8 us                                                | 16.5 us: 1.19x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.84 ms: 1.47x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.6 ms: 1.28x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 114 us: 4.55x faster                                                             |
| generators                 | 74.9 ms                                                | 29.6 ms: 2.53x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 496 ms: 1.76x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.72x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.6 ms: 1.25x faster                                                            |
| coroutines                 | 27.0 ms                                                | 21.9 ms: 1.24x faster                                                            |
| async_tree_none            | 528 ms                                                 | 452 ms: 1.17x faster                                                             |
| richards_super             | 61.9 ms                                                | 53.7 ms: 1.15x faster                                                            |
| comprehensions             | 23.6 us                                                | 20.5 us: 1.15x faster                                                            |
| logging_silent             | 111 ns                                                 | 99.1 ns: 1.12x faster                                                            |
| deltablue                  | 3.92 ms                                                | 3.52 ms: 1.11x faster                                                            |
| unpack_sequence            | 43.5 ns                                                | 39.2 ns: 1.11x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 578 ms: 1.11x faster                                                             |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.08x faster                                                            |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 459 ms: 1.07x faster                                                             |
| pickle_pure_python         | 320 us                                                 | 299 us: 1.07x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.07x faster                                                           |
| logging_simple             | 6.22 us                                                | 5.85 us: 1.06x faster                                                            |
| sqlglot_transpile          | 1.75 ms                                                | 1.66 ms: 1.06x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.05x faster                                                             |
| unpickle_list              | 5.21 us                                                | 4.96 us: 1.05x faster                                                            |
| raytrace                   | 309 ms                                                 | 296 ms: 1.04x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 603 ms: 1.04x faster                                                             |
| sympy_integrate            | 21.5 ms                                                | 20.7 ms: 1.04x faster                                                            |
| richards                   | 49.8 ms                                                | 48.0 ms: 1.04x faster                                                            |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                             |
| unpickle_pure_python       | 242 us                                                 | 234 us: 1.03x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 737 ms: 1.03x faster                                                             |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 727 ms: 1.03x faster                                                             |
| sympy_str                  | 297 ms                                                 | 289 ms: 1.03x faster                                                             |
| logging_format             | 6.81 us                                                | 6.67 us: 1.02x faster                                                            |
| gc_traversal               | 4.01 ms                                                | 3.93 ms: 1.02x faster                                                            |
| deepcopy                   | 365 us                                                 | 359 us: 1.02x faster                                                             |
| json_loads                 | 29.2 us                                                | 28.7 us: 1.02x faster                                                            |
| deepcopy_reduce            | 3.22 us                                                | 3.16 us: 1.02x faster                                                            |
| pathlib                    | 18.5 ms                                                | 18.7 ms: 1.01x slower                                                            |
| scimark_lu                 | 116 ms                                                 | 117 ms: 1.01x slower                                                             |
| bench_thread_pool          | 834 us                                                 | 843 us: 1.01x slower                                                             |
| sqlglot_normalize          | 113 ms                                                 | 114 ms: 1.01x slower                                                             |
| scimark_sor                | 121 ms                                                 | 123 ms: 1.01x slower                                                             |
| dask                       | 365 ms                                                 | 369 ms: 1.01x slower                                                             |
| docutils                   | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                           |
| xml_etree_iterparse        | 108 ms                                                 | 109 ms: 1.01x slower                                                             |
| pickle_dict                | 34.6 us                                                | 35.1 us: 1.01x slower                                                            |
| pycparser                  | 1.19 sec                                               | 1.21 sec: 1.02x slower                                                           |
| tomli_loads                | 2.30 sec                                               | 2.35 sec: 1.02x slower                                                           |
| sqlglot_optimize           | 55.3 ms                                                | 57.4 ms: 1.04x slower                                                            |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                                            |
| regex_effbot               | 3.51 ms                                                | 3.66 ms: 1.04x slower                                                            |
| meteor_contest             | 109 ms                                                 | 114 ms: 1.05x slower                                                             |
| regex_compile              | 141 ms                                                 | 149 ms: 1.05x slower                                                             |
| pickle                     | 11.0 us                                                | 11.6 us: 1.05x slower                                                            |
| nqueens                    | 87.9 ms                                                | 92.8 ms: 1.06x slower                                                            |
| regex_v8                   | 22.9 ms                                                | 24.2 ms: 1.06x slower                                                            |
| xml_etree_process          | 56.9 ms                                                | 60.4 ms: 1.06x slower                                                            |
| dulwich_log                | 64.6 ms                                                | 68.6 ms: 1.06x slower                                                            |
| 2to3                       | 264 ms                                                 | 282 ms: 1.07x slower                                                             |
| pprint_safe_repr           | 747 ms                                                 | 799 ms: 1.07x slower                                                             |
| pprint_pformat             | 1.55 sec                                               | 1.67 sec: 1.07x slower                                                           |
| regex_dna                  | 205 ms                                                 | 221 ms: 1.08x slower                                                             |
| chameleon                  | 6.70 ms                                                | 7.27 ms: 1.08x slower                                                            |
| crypto_pyaes               | 76.7 ms                                                | 84.0 ms: 1.09x slower                                                            |
| xml_etree_generate         | 81.1 ms                                                | 88.9 ms: 1.10x slower                                                            |
| fannkuch                   | 405 ms                                                 | 448 ms: 1.10x slower                                                             |
| sqlite_synth               | 2.57 us                                                | 2.85 us: 1.11x slower                                                            |
| pickle_list                | 4.59 us                                                | 5.12 us: 1.12x slower                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.63 ms: 1.12x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 79.8 ms: 1.13x slower                                                            |
| float                      | 78.9 ms                                                | 92.0 ms: 1.17x slower                                                            |
| pyflate                    | 434 ms                                                 | 509 ms: 1.17x slower                                                             |
| unpickle                   | 13.8 us                                                | 16.5 us: 1.19x slower                                                            |
| go                         | 149 ms                                                 | 177 ms: 1.19x slower                                                             |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| scimark_fft                | 345 ms                                                 | 416 ms: 1.21x slower                                                             |
| coverage                   | 78.8 ms                                                | 95.1 ms: 1.21x slower                                                            |
| hexiom                     | 6.89 ms                                                | 8.34 ms: 1.21x slower                                                            |
| async_generators           | 374 ms                                                 | 456 ms: 1.22x slower                                                             |
| nbody                      | 96.0 ms                                                | 119 ms: 1.24x slower                                                             |
| spectral_norm              | 108 ms                                                 | 135 ms: 1.25x slower                                                             |
| mypy2                      | 686 ms                                                 | 870 ms: 1.27x slower                                                             |
| telco                      | 6.86 ms                                                | 8.75 ms: 1.28x slower                                                            |
| mako                       | 10.7 ms                                                | 13.6 ms: 1.28x slower                                                            |
| python_startup_no_site     | 6.01 ms                                                | 8.84 ms: 1.47x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (8): chaos, bench_mp_pool, deepcopy_memo, json, asyncio_websockets, sympy_expand, tornado_http, mdp
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 93.47% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x