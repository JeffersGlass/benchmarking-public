
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 27ce303
- commit date: 2024-01-20
- overall geometric mean: 1.00x slower
- HPT reliability: 94.89%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.28x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 287 ms: 1.09x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.39 ms: 1.10x slower                                                            |
| docutils       | 2.66 sec                                               | 2.72 sec: 1.02x slower                                                           |
| tornado_http   | 98.1 ms                                                | 97.5 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 449 ms: 1.18x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 578 ms: 1.11x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 576 ms: 1.09x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 460 ms: 1.07x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.07x faster                                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 721 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 736 ms: 1.03x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| float          | 78.9 ms                                                | 89.4 ms: 1.13x slower                                                            |
| nbody          | 96.0 ms                                                | 119 ms: 1.24x slower                                                             |
| Geometric mean | (ref)                                                  | 1.11x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.65 ms: 1.04x slower                                                            |
| regex_compile  | 141 ms                                                 | 150 ms: 1.06x slower                                                             |
| regex_dna      | 205 ms                                                 | 227 ms: 1.11x slower                                                             |
| regex_v8       | 22.9 ms                                                | 25.9 ms: 1.13x slower                                                            |
| Geometric mean | (ref)                                                  | 1.09x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 305 us: 1.05x faster                                                             |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.05x faster                                                             |
| unpickle_list        | 5.21 us                                                | 5.01 us: 1.04x faster                                                            |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                                            |
| unpickle_pure_python | 242 us                                                 | 238 us: 1.01x faster                                                             |
| pickle_dict          | 34.6 us                                                | 34.8 us: 1.01x slower                                                            |
| tomli_loads          | 2.30 sec                                               | 2.32 sec: 1.01x slower                                                           |
| xml_etree_iterparse  | 108 ms                                                 | 109 ms: 1.01x slower                                                             |
| xml_etree_process    | 56.9 ms                                                | 61.2 ms: 1.08x slower                                                            |
| pickle               | 11.0 us                                                | 11.9 us: 1.09x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 89.6 ms: 1.11x slower                                                            |
| unpickle             | 13.8 us                                                | 15.3 us: 1.11x slower                                                            |
| pickle_list          | 4.59 us                                                | 5.25 us: 1.14x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.77 ms: 1.46x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.7 ms: 1.28x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 120 us: 4.34x faster                                                             |
| generators                 | 74.9 ms                                                | 29.7 ms: 2.52x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 500 ms: 1.75x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.72x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                            |
| coroutines                 | 27.0 ms                                                | 22.2 ms: 1.22x faster                                                            |
| async_tree_none            | 528 ms                                                 | 449 ms: 1.18x faster                                                             |
| richards_super             | 61.9 ms                                                | 54.5 ms: 1.14x faster                                                            |
| comprehensions             | 23.6 us                                                | 21.1 us: 1.12x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 578 ms: 1.11x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 576 ms: 1.09x faster                                                             |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.07x faster                                                            |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 460 ms: 1.07x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.07x faster                                                           |
| logging_silent             | 111 ns                                                 | 105 ns: 1.06x faster                                                             |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.05x faster                                                             |
| pickle_pure_python         | 320 us                                                 | 305 us: 1.05x faster                                                             |
| sqlglot_transpile          | 1.75 ms                                                | 1.67 ms: 1.05x faster                                                            |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.05x faster                                                             |
| logging_simple             | 6.22 us                                                | 5.96 us: 1.04x faster                                                            |
| raytrace                   | 309 ms                                                 | 296 ms: 1.04x faster                                                             |
| unpickle_list              | 5.21 us                                                | 5.01 us: 1.04x faster                                                            |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 721 ms: 1.04x faster                                                             |
| json_loads                 | 29.2 us                                                | 28.1 us: 1.04x faster                                                            |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 736 ms: 1.03x faster                                                             |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| richards                   | 49.8 ms                                                | 48.4 ms: 1.03x faster                                                            |
| sympy_integrate            | 21.5 ms                                                | 20.9 ms: 1.03x faster                                                            |
| sympy_str                  | 297 ms                                                 | 292 ms: 1.02x faster                                                             |
| unpickle_pure_python       | 242 us                                                 | 238 us: 1.01x faster                                                             |
| json                       | 5.24 ms                                                | 5.17 ms: 1.01x faster                                                            |
| pathlib                    | 18.5 ms                                                | 18.3 ms: 1.01x faster                                                            |
| deepcopy_reduce            | 3.22 us                                                | 3.17 us: 1.01x faster                                                            |
| deepcopy                   | 365 us                                                 | 361 us: 1.01x faster                                                             |
| chaos                      | 71.9 ms                                                | 71.3 ms: 1.01x faster                                                            |
| gc_traversal               | 4.01 ms                                                | 3.98 ms: 1.01x faster                                                            |
| logging_format             | 6.81 us                                                | 6.77 us: 1.01x faster                                                            |
| tornado_http               | 98.1 ms                                                | 97.5 ms: 1.01x faster                                                            |
| pickle_dict                | 34.6 us                                                | 34.8 us: 1.01x slower                                                            |
| tomli_loads                | 2.30 sec                                               | 2.32 sec: 1.01x slower                                                           |
| xml_etree_iterparse        | 108 ms                                                 | 109 ms: 1.01x slower                                                             |
| dask                       | 365 ms                                                 | 369 ms: 1.01x slower                                                             |
| sympy_expand               | 484 ms                                                 | 492 ms: 1.02x slower                                                             |
| scimark_lu                 | 116 ms                                                 | 118 ms: 1.02x slower                                                             |
| bench_thread_pool          | 834 us                                                 | 850 us: 1.02x slower                                                             |
| pycparser                  | 1.19 sec                                               | 1.21 sec: 1.02x slower                                                           |
| mdp                        | 2.77 sec                                               | 2.83 sec: 1.02x slower                                                           |
| docutils                   | 2.66 sec                                               | 2.72 sec: 1.02x slower                                                           |
| create_gc_cycles           | 1.43 ms                                                | 1.46 ms: 1.02x slower                                                            |
| sqlglot_normalize          | 113 ms                                                 | 116 ms: 1.03x slower                                                             |
| deepcopy_memo              | 40.2 us                                                | 41.2 us: 1.03x slower                                                            |
| regex_effbot               | 3.51 ms                                                | 3.65 ms: 1.04x slower                                                            |
| meteor_contest             | 109 ms                                                 | 114 ms: 1.04x slower                                                             |
| sqlglot_optimize           | 55.3 ms                                                | 58.4 ms: 1.06x slower                                                            |
| go                         | 149 ms                                                 | 157 ms: 1.06x slower                                                             |
| dulwich_log                | 64.6 ms                                                | 68.6 ms: 1.06x slower                                                            |
| regex_compile              | 141 ms                                                 | 150 ms: 1.06x slower                                                             |
| nqueens                    | 87.9 ms                                                | 93.8 ms: 1.07x slower                                                            |
| xml_etree_process          | 56.9 ms                                                | 61.2 ms: 1.08x slower                                                            |
| pprint_safe_repr           | 747 ms                                                 | 810 ms: 1.08x slower                                                             |
| pprint_pformat             | 1.55 sec                                               | 1.69 sec: 1.09x slower                                                           |
| 2to3                       | 264 ms                                                 | 287 ms: 1.09x slower                                                             |
| pickle                     | 11.0 us                                                | 11.9 us: 1.09x slower                                                            |
| fannkuch                   | 405 ms                                                 | 442 ms: 1.09x slower                                                             |
| crypto_pyaes               | 76.7 ms                                                | 84.0 ms: 1.10x slower                                                            |
| chameleon                  | 6.70 ms                                                | 7.39 ms: 1.10x slower                                                            |
| xml_etree_generate         | 81.1 ms                                                | 89.6 ms: 1.11x slower                                                            |
| unpickle                   | 13.8 us                                                | 15.3 us: 1.11x slower                                                            |
| scimark_sor                | 121 ms                                                 | 134 ms: 1.11x slower                                                             |
| regex_dna                  | 205 ms                                                 | 227 ms: 1.11x slower                                                             |
| sqlite_synth               | 2.57 us                                                | 2.86 us: 1.11x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 79.5 ms: 1.12x slower                                                            |
| regex_v8                   | 22.9 ms                                                | 25.9 ms: 1.13x slower                                                            |
| float                      | 78.9 ms                                                | 89.4 ms: 1.13x slower                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.72 ms: 1.14x slower                                                            |
| pickle_list                | 4.59 us                                                | 5.25 us: 1.14x slower                                                            |
| deltablue                  | 3.92 ms                                                | 4.59 ms: 1.17x slower                                                            |
| hexiom                     | 6.89 ms                                                | 8.15 ms: 1.18x slower                                                            |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                            |
| pyflate                    | 434 ms                                                 | 522 ms: 1.20x slower                                                             |
| coverage                   | 78.8 ms                                                | 95.2 ms: 1.21x slower                                                            |
| scimark_fft                | 345 ms                                                 | 422 ms: 1.22x slower                                                             |
| async_generators           | 374 ms                                                 | 459 ms: 1.23x slower                                                             |
| nbody                      | 96.0 ms                                                | 119 ms: 1.24x slower                                                             |
| mypy2                      | 686 ms                                                 | 863 ms: 1.26x slower                                                             |
| spectral_norm              | 108 ms                                                 | 138 ms: 1.28x slower                                                             |
| mako                       | 10.7 ms                                                | 13.7 ms: 1.28x slower                                                            |
| telco                      | 6.86 ms                                                | 8.82 ms: 1.29x slower                                                            |
| unpack_sequence            | 43.5 ns                                                | 56.7 ns: 1.31x slower                                                            |
| python_startup_no_site     | 6.01 ms                                                | 8.77 ms: 1.46x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (2): asyncio_websockets, bench_mp_pool
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 94.89% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.28x