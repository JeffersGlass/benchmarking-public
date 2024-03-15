
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.02x faster
- HPT reliability: 57.97%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 280 ms: 1.06x slower                                                             |
| chameleon      | 6.70 ms                                                | 6.96 ms: 1.04x slower                                                            |
| docutils       | 2.66 sec                                               | 2.68 sec: 1.01x slower                                                           |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 442 ms: 1.19x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 570 ms: 1.12x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 453 ms: 1.08x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 580 ms: 1.08x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 724 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 717 ms: 1.05x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.09x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| nbody          | 96.0 ms                                                | 99.8 ms: 1.04x slower                                                            |
| float          | 78.9 ms                                                | 86.6 ms: 1.10x slower                                                            |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 143 ms: 1.01x slower                                                             |
| regex_effbot   | 3.51 ms                                                | 3.67 ms: 1.05x slower                                                            |
| regex_dna      | 205 ms                                                 | 222 ms: 1.08x slower                                                             |
| regex_v8       | 22.9 ms                                                | 25.2 ms: 1.10x slower                                                            |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 300 us: 1.07x faster                                                             |
| unpickle_pure_python | 242 us                                                 | 229 us: 1.06x faster                                                             |
| tomli_loads          | 2.30 sec                                               | 2.22 sec: 1.04x faster                                                           |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                             |
| json_loads           | 29.2 us                                                | 28.2 us: 1.03x faster                                                            |
| xml_etree_iterparse  | 108 ms                                                 | 109 ms: 1.01x slower                                                             |
| pickle_dict          | 34.6 us                                                | 35.0 us: 1.01x slower                                                            |
| xml_etree_process    | 56.9 ms                                                | 59.4 ms: 1.04x slower                                                            |
| pickle               | 11.0 us                                                | 11.6 us: 1.06x slower                                                            |
| unpickle             | 13.8 us                                                | 14.7 us: 1.06x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 87.7 ms: 1.08x slower                                                            |
| pickle_list          | 4.59 us                                                | 5.20 us: 1.13x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.3 ms: 1.20x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.93 ms: 1.49x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.34x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 12.5 ms: 1.17x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 111 us: 4.67x faster                                                             |
| generators                 | 74.9 ms                                                | 29.7 ms: 2.52x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 495 ms: 1.77x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.81 sec: 1.72x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                            |
| comprehensions             | 23.6 us                                                | 19.4 us: 1.22x faster                                                            |
| async_tree_none            | 528 ms                                                 | 442 ms: 1.19x faster                                                             |
| richards_super             | 61.9 ms                                                | 52.9 ms: 1.17x faster                                                            |
| coroutines                 | 27.0 ms                                                | 23.2 ms: 1.17x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 570 ms: 1.12x faster                                                             |
| sqlglot_parse              | 1.43 ms                                                | 1.29 ms: 1.11x faster                                                            |
| raytrace                   | 309 ms                                                 | 281 ms: 1.10x faster                                                             |
| logging_silent             | 111 ns                                                 | 102 ns: 1.09x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 453 ms: 1.08x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 580 ms: 1.08x faster                                                             |
| sqlglot_transpile          | 1.75 ms                                                | 1.62 ms: 1.08x faster                                                            |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                           |
| richards                   | 49.8 ms                                                | 46.6 ms: 1.07x faster                                                            |
| pickle_pure_python         | 320 us                                                 | 300 us: 1.07x faster                                                             |
| logging_format             | 6.81 us                                                | 6.40 us: 1.06x faster                                                            |
| logging_simple             | 6.22 us                                                | 5.86 us: 1.06x faster                                                            |
| unpickle_pure_python       | 242 us                                                 | 229 us: 1.06x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 724 ms: 1.05x faster                                                             |
| deepcopy                   | 365 us                                                 | 349 us: 1.05x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 717 ms: 1.05x faster                                                             |
| deepcopy_reduce            | 3.22 us                                                | 3.08 us: 1.04x faster                                                            |
| tomli_loads                | 2.30 sec                                               | 2.22 sec: 1.04x faster                                                           |
| sympy_sum                  | 169 ms                                                 | 162 ms: 1.04x faster                                                             |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                             |
| gc_traversal               | 4.01 ms                                                | 3.87 ms: 1.04x faster                                                            |
| deepcopy_memo              | 40.2 us                                                | 38.8 us: 1.04x faster                                                            |
| json_loads                 | 29.2 us                                                | 28.2 us: 1.03x faster                                                            |
| chaos                      | 71.9 ms                                                | 69.5 ms: 1.03x faster                                                            |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| scimark_lu                 | 116 ms                                                 | 113 ms: 1.03x faster                                                             |
| sympy_str                  | 297 ms                                                 | 291 ms: 1.02x faster                                                             |
| pathlib                    | 18.5 ms                                                | 18.2 ms: 1.02x faster                                                            |
| pycparser                  | 1.19 sec                                               | 1.17 sec: 1.02x faster                                                           |
| sqlglot_normalize          | 113 ms                                                 | 111 ms: 1.02x faster                                                             |
| mdp                        | 2.77 sec                                               | 2.74 sec: 1.01x faster                                                           |
| json                       | 5.24 ms                                                | 5.19 ms: 1.01x faster                                                            |
| sympy_integrate            | 21.5 ms                                                | 21.3 ms: 1.01x faster                                                            |
| bench_thread_pool          | 834 us                                                 | 839 us: 1.00x slower                                                             |
| docutils                   | 2.66 sec                                               | 2.68 sec: 1.01x slower                                                           |
| asyncio_websockets         | 550 ms                                                 | 555 ms: 1.01x slower                                                             |
| xml_etree_iterparse        | 108 ms                                                 | 109 ms: 1.01x slower                                                             |
| pickle_dict                | 34.6 us                                                | 35.0 us: 1.01x slower                                                            |
| regex_compile              | 141 ms                                                 | 143 ms: 1.01x slower                                                             |
| sqlglot_optimize           | 55.3 ms                                                | 56.5 ms: 1.02x slower                                                            |
| go                         | 149 ms                                                 | 152 ms: 1.02x slower                                                             |
| deltablue                  | 3.92 ms                                                | 4.01 ms: 1.02x slower                                                            |
| nqueens                    | 87.9 ms                                                | 90.0 ms: 1.02x slower                                                            |
| scimark_sor                | 121 ms                                                 | 125 ms: 1.03x slower                                                             |
| meteor_contest             | 109 ms                                                 | 112 ms: 1.03x slower                                                             |
| chameleon                  | 6.70 ms                                                | 6.96 ms: 1.04x slower                                                            |
| nbody                      | 96.0 ms                                                | 99.8 ms: 1.04x slower                                                            |
| xml_etree_process          | 56.9 ms                                                | 59.4 ms: 1.04x slower                                                            |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.05x slower                                                            |
| regex_effbot               | 3.51 ms                                                | 3.67 ms: 1.05x slower                                                            |
| pickle                     | 11.0 us                                                | 11.6 us: 1.06x slower                                                            |
| crypto_pyaes               | 76.7 ms                                                | 81.1 ms: 1.06x slower                                                            |
| fannkuch                   | 405 ms                                                 | 428 ms: 1.06x slower                                                             |
| 2to3                       | 264 ms                                                 | 280 ms: 1.06x slower                                                             |
| dulwich_log                | 64.6 ms                                                | 68.5 ms: 1.06x slower                                                            |
| unpickle                   | 13.8 us                                                | 14.7 us: 1.06x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 76.2 ms: 1.08x slower                                                            |
| scimark_fft                | 345 ms                                                 | 372 ms: 1.08x slower                                                             |
| xml_etree_generate         | 81.1 ms                                                | 87.7 ms: 1.08x slower                                                            |
| pprint_safe_repr           | 747 ms                                                 | 809 ms: 1.08x slower                                                             |
| regex_dna                  | 205 ms                                                 | 222 ms: 1.08x slower                                                             |
| float                      | 78.9 ms                                                | 86.6 ms: 1.10x slower                                                            |
| sqlite_synth               | 2.57 us                                                | 2.82 us: 1.10x slower                                                            |
| regex_v8                   | 22.9 ms                                                | 25.2 ms: 1.10x slower                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.57 ms: 1.11x slower                                                            |
| pprint_pformat             | 1.55 sec                                               | 1.73 sec: 1.11x slower                                                           |
| pickle_list                | 4.59 us                                                | 5.20 us: 1.13x slower                                                            |
| mako                       | 10.7 ms                                                | 12.5 ms: 1.17x slower                                                            |
| pyflate                    | 434 ms                                                 | 515 ms: 1.19x slower                                                             |
| python_startup             | 8.56 ms                                                | 10.3 ms: 1.20x slower                                                            |
| coverage                   | 78.8 ms                                                | 94.6 ms: 1.20x slower                                                            |
| telco                      | 6.86 ms                                                | 8.43 ms: 1.23x slower                                                            |
| async_generators           | 374 ms                                                 | 463 ms: 1.24x slower                                                             |
| spectral_norm              | 108 ms                                                 | 135 ms: 1.24x slower                                                             |
| hexiom                     | 6.89 ms                                                | 8.65 ms: 1.26x slower                                                            |
| mypy2                      | 686 ms                                                 | 871 ms: 1.27x slower                                                             |
| python_startup_no_site     | 6.01 ms                                                | 8.93 ms: 1.49x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                                     |

Benchmark hidden because not significant (6): unpack_sequence, tornado_http, bench_mp_pool, dask, unpickle_list, sympy_expand
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 57.97% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.03x