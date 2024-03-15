
# Results vs. 3.11.0

- fork: faster-cpython
- ref: tier_2_inline_consts
- machine: linux-x86_64
- commit hash: 9d22a48
- commit date: 2024-01-17
- overall geometric mean: 1.01x faster
- HPT reliability: 94.21%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 281 ms: 1.06x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.35 ms: 1.10x slower                                                            |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.02x slower                                                           |
| tornado_http   | 98.1 ms                                                | 99.7 ms: 1.02x slower                                                            |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 447 ms: 1.18x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 572 ms: 1.12x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 454 ms: 1.08x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 585 ms: 1.07x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 728 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 716 ms: 1.05x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.09x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                             |
| float          | 78.9 ms                                                | 89.9 ms: 1.14x slower                                                            |
| nbody          | 96.0 ms                                                | 114 ms: 1.18x slower                                                             |
| Geometric mean | (ref)                                                  | 1.09x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.63 ms: 1.04x slower                                                            |
| regex_compile  | 141 ms                                                 | 149 ms: 1.05x slower                                                             |
| regex_dna      | 205 ms                                                 | 226 ms: 1.11x slower                                                             |
| regex_v8       | 22.9 ms                                                | 27.0 ms: 1.18x slower                                                            |
| Geometric mean | (ref)                                                  | 1.09x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 301 us: 1.06x faster                                                             |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                                            |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                                             |
| unpickle_pure_python | 242 us                                                 | 234 us: 1.03x faster                                                             |
| unpickle_list        | 5.21 us                                                | 5.13 us: 1.02x faster                                                            |
| pickle_dict          | 34.6 us                                                | 34.1 us: 1.02x faster                                                            |
| tomli_loads          | 2.30 sec                                               | 2.34 sec: 1.02x slower                                                           |
| xml_etree_iterparse  | 108 ms                                                 | 110 ms: 1.02x slower                                                             |
| pickle               | 11.0 us                                                | 11.5 us: 1.05x slower                                                            |
| xml_etree_process    | 56.9 ms                                                | 60.5 ms: 1.06x slower                                                            |
| unpickle             | 13.8 us                                                | 15.0 us: 1.09x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 89.0 ms: 1.10x slower                                                            |
| pickle_list          | 4.59 us                                                | 5.14 us: 1.12x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.00x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.75 ms: 1.46x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.3 ms: 1.25x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 116 us: 4.49x faster                                                             |
| generators                 | 74.9 ms                                                | 29.1 ms: 2.57x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 497 ms: 1.76x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                            |
| coroutines                 | 27.0 ms                                                | 22.2 ms: 1.22x faster                                                            |
| async_tree_none            | 528 ms                                                 | 447 ms: 1.18x faster                                                             |
| comprehensions             | 23.6 us                                                | 20.4 us: 1.16x faster                                                            |
| richards_super             | 61.9 ms                                                | 54.2 ms: 1.14x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 572 ms: 1.12x faster                                                             |
| unpack_sequence            | 43.5 ns                                                | 39.7 ns: 1.09x faster                                                            |
| sqlglot_parse              | 1.43 ms                                                | 1.32 ms: 1.09x faster                                                            |
| gc_traversal               | 4.01 ms                                                | 3.70 ms: 1.08x faster                                                            |
| async_tree_none_tg         | 491 ms                                                 | 454 ms: 1.08x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 585 ms: 1.07x faster                                                             |
| pickle_pure_python         | 320 us                                                 | 301 us: 1.06x faster                                                             |
| sqlglot_transpile          | 1.75 ms                                                | 1.65 ms: 1.06x faster                                                            |
| logging_silent             | 111 ns                                                 | 106 ns: 1.05x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 728 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 716 ms: 1.05x faster                                                             |
| raytrace                   | 309 ms                                                 | 296 ms: 1.04x faster                                                             |
| richards                   | 49.8 ms                                                | 47.9 ms: 1.04x faster                                                            |
| json_loads                 | 29.2 us                                                | 28.1 us: 1.04x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 163 ms: 1.04x faster                                                             |
| mdp                        | 2.77 sec                                               | 2.68 sec: 1.04x faster                                                           |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                                             |
| unpickle_pure_python       | 242 us                                                 | 234 us: 1.03x faster                                                             |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                             |
| sympy_str                  | 297 ms                                                 | 291 ms: 1.02x faster                                                             |
| logging_simple             | 6.22 us                                                | 6.09 us: 1.02x faster                                                            |
| unpickle_list              | 5.21 us                                                | 5.13 us: 1.02x faster                                                            |
| json                       | 5.24 ms                                                | 5.16 ms: 1.02x faster                                                            |
| pickle_dict                | 34.6 us                                                | 34.1 us: 1.02x faster                                                            |
| sympy_integrate            | 21.5 ms                                                | 21.2 ms: 1.01x faster                                                            |
| deepcopy_reduce            | 3.22 us                                                | 3.20 us: 1.01x faster                                                            |
| deepcopy                   | 365 us                                                 | 364 us: 1.00x faster                                                             |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                             |
| sympy_expand               | 484 ms                                                 | 487 ms: 1.01x slower                                                             |
| logging_format             | 6.81 us                                                | 6.86 us: 1.01x slower                                                            |
| sqlglot_normalize          | 113 ms                                                 | 114 ms: 1.01x slower                                                             |
| pathlib                    | 18.5 ms                                                | 18.7 ms: 1.01x slower                                                            |
| dask                       | 365 ms                                                 | 370 ms: 1.01x slower                                                             |
| tomli_loads                | 2.30 sec                                               | 2.34 sec: 1.02x slower                                                           |
| docutils                   | 2.66 sec                                               | 2.70 sec: 1.02x slower                                                           |
| tornado_http               | 98.1 ms                                                | 99.7 ms: 1.02x slower                                                            |
| bench_thread_pool          | 834 us                                                 | 850 us: 1.02x slower                                                             |
| xml_etree_iterparse        | 108 ms                                                 | 110 ms: 1.02x slower                                                             |
| deepcopy_memo              | 40.2 us                                                | 41.2 us: 1.03x slower                                                            |
| nqueens                    | 87.9 ms                                                | 91.0 ms: 1.04x slower                                                            |
| regex_effbot               | 3.51 ms                                                | 3.63 ms: 1.04x slower                                                            |
| meteor_contest             | 109 ms                                                 | 113 ms: 1.04x slower                                                             |
| go                         | 149 ms                                                 | 154 ms: 1.04x slower                                                             |
| sqlglot_optimize           | 55.3 ms                                                | 57.6 ms: 1.04x slower                                                            |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.04x slower                                                            |
| pickle                     | 11.0 us                                                | 11.5 us: 1.05x slower                                                            |
| regex_compile              | 141 ms                                                 | 149 ms: 1.05x slower                                                             |
| 2to3                       | 264 ms                                                 | 281 ms: 1.06x slower                                                             |
| crypto_pyaes               | 76.7 ms                                                | 81.5 ms: 1.06x slower                                                            |
| xml_etree_process          | 56.9 ms                                                | 60.5 ms: 1.06x slower                                                            |
| dulwich_log                | 64.6 ms                                                | 69.5 ms: 1.08x slower                                                            |
| fannkuch                   | 405 ms                                                 | 439 ms: 1.08x slower                                                             |
| scimark_sor                | 121 ms                                                 | 132 ms: 1.08x slower                                                             |
| unpickle                   | 13.8 us                                                | 15.0 us: 1.09x slower                                                            |
| chameleon                  | 6.70 ms                                                | 7.35 ms: 1.10x slower                                                            |
| xml_etree_generate         | 81.1 ms                                                | 89.0 ms: 1.10x slower                                                            |
| pprint_pformat             | 1.55 sec                                               | 1.71 sec: 1.10x slower                                                           |
| pprint_safe_repr           | 747 ms                                                 | 824 ms: 1.10x slower                                                             |
| regex_dna                  | 205 ms                                                 | 226 ms: 1.11x slower                                                             |
| sqlite_synth               | 2.57 us                                                | 2.86 us: 1.11x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 78.9 ms: 1.12x slower                                                            |
| pickle_list                | 4.59 us                                                | 5.14 us: 1.12x slower                                                            |
| float                      | 78.9 ms                                                | 89.9 ms: 1.14x slower                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.75 ms: 1.14x slower                                                            |
| deltablue                  | 3.92 ms                                                | 4.49 ms: 1.15x slower                                                            |
| hexiom                     | 6.89 ms                                                | 8.04 ms: 1.17x slower                                                            |
| pyflate                    | 434 ms                                                 | 509 ms: 1.17x slower                                                             |
| regex_v8                   | 22.9 ms                                                | 27.0 ms: 1.18x slower                                                            |
| nbody                      | 96.0 ms                                                | 114 ms: 1.18x slower                                                             |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                            |
| coverage                   | 78.8 ms                                                | 94.8 ms: 1.20x slower                                                            |
| async_generators           | 374 ms                                                 | 454 ms: 1.21x slower                                                             |
| mako                       | 10.7 ms                                                | 13.3 ms: 1.25x slower                                                            |
| mypy2                      | 686 ms                                                 | 862 ms: 1.26x slower                                                             |
| telco                      | 6.86 ms                                                | 8.68 ms: 1.27x slower                                                            |
| scimark_fft                | 345 ms                                                 | 442 ms: 1.28x slower                                                             |
| spectral_norm              | 108 ms                                                 | 139 ms: 1.29x slower                                                             |
| python_startup_no_site     | 6.01 ms                                                | 8.75 ms: 1.46x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (4): bench_mp_pool, chaos, pycparser, scimark_lu
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 94.21% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x