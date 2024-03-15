
# Results vs. 3.11.0

- fork: faster-cpython
- ref: abstract_interpreter
- machine: linux-x86_64
- commit hash: 9f32fb0
- commit date: 2024-02-03
- overall geometric mean: 1.01x faster \*
- HPT reliability: 89.85%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 284 ms: 1.07x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.28 ms: 1.09x slower                                                            |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                           |
| tornado_http   | 98.1 ms                                                | 99.0 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 448 ms: 1.18x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 575 ms: 1.11x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 458 ms: 1.07x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 586 ms: 1.07x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 729 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 717 ms: 1.04x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| nbody          | 96.0 ms                                                | 109 ms: 1.13x slower                                                             |
| float          | 78.9 ms                                                | 90.0 ms: 1.14x slower                                                            |
| Geometric mean | (ref)                                                  | 1.08x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.67 ms: 1.05x slower                                                            |
| regex_compile  | 141 ms                                                 | 149 ms: 1.06x slower                                                             |
| regex_dna      | 205 ms                                                 | 220 ms: 1.08x slower                                                             |
| regex_v8       | 22.9 ms                                                | 25.0 ms: 1.09x slower                                                            |
| Geometric mean | (ref)                                                  | 1.07x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.7 ms: 1.25x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 301 us: 1.06x faster                                                             |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                                             |
| unpickle_list        | 5.21 us                                                | 5.02 us: 1.04x faster                                                            |
| unpickle_pure_python | 242 us                                                 | 234 us: 1.03x faster                                                             |
| json_loads           | 29.2 us                                                | 28.6 us: 1.02x faster                                                            |
| xml_etree_process    | 56.9 ms                                                | 60.1 ms: 1.06x slower                                                            |
| pickle               | 11.0 us                                                | 11.7 us: 1.07x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 88.3 ms: 1.09x slower                                                            |
| tomli_loads          | 2.30 sec                                               | 2.55 sec: 1.11x slower                                                           |
| pickle_list          | 4.59 us                                                | 5.26 us: 1.15x slower                                                            |
| unpickle             | 13.8 us                                                | 16.3 us: 1.18x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (2): pickle_dict, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.80 ms: 1.46x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.1 ms: 1.23x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 112 us: 4.66x faster                                                             |
| generators                 | 74.9 ms                                                | 30.3 ms: 2.47x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 491 ms: 1.78x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.72x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.7 ms: 1.25x faster                                                            |
| coroutines                 | 27.0 ms                                                | 22.0 ms: 1.23x faster                                                            |
| async_tree_none            | 528 ms                                                 | 448 ms: 1.18x faster                                                             |
| comprehensions             | 23.6 us                                                | 20.8 us: 1.14x faster                                                            |
| richards_super             | 61.9 ms                                                | 54.5 ms: 1.14x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 575 ms: 1.11x faster                                                             |
| deltablue                  | 3.92 ms                                                | 3.54 ms: 1.11x faster                                                            |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.08x faster                                                            |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 458 ms: 1.07x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 586 ms: 1.07x faster                                                             |
| pickle_pure_python         | 320 us                                                 | 301 us: 1.06x faster                                                             |
| logging_simple             | 6.22 us                                                | 5.85 us: 1.06x faster                                                            |
| gc_traversal               | 4.01 ms                                                | 3.79 ms: 1.06x faster                                                            |
| logging_silent             | 111 ns                                                 | 105 ns: 1.06x faster                                                             |
| sqlglot_transpile          | 1.75 ms                                                | 1.66 ms: 1.05x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 729 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 717 ms: 1.04x faster                                                             |
| mdp                        | 2.77 sec                                               | 2.66 sec: 1.04x faster                                                           |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.04x faster                                                             |
| unpickle_list              | 5.21 us                                                | 5.02 us: 1.04x faster                                                            |
| unpickle_pure_python       | 242 us                                                 | 234 us: 1.03x faster                                                             |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| logging_format             | 6.81 us                                                | 6.63 us: 1.03x faster                                                            |
| sympy_integrate            | 21.5 ms                                                | 20.9 ms: 1.03x faster                                                            |
| raytrace                   | 309 ms                                                 | 301 ms: 1.03x faster                                                             |
| deepcopy_reduce            | 3.22 us                                                | 3.14 us: 1.03x faster                                                            |
| richards                   | 49.8 ms                                                | 48.8 ms: 1.02x faster                                                            |
| deepcopy                   | 365 us                                                 | 358 us: 1.02x faster                                                             |
| json_loads                 | 29.2 us                                                | 28.6 us: 1.02x faster                                                            |
| deepcopy_memo              | 40.2 us                                                | 39.6 us: 1.01x faster                                                            |
| sympy_str                  | 297 ms                                                 | 293 ms: 1.01x faster                                                             |
| chaos                      | 71.9 ms                                                | 72.2 ms: 1.00x slower                                                            |
| scimark_sor                | 121 ms                                                 | 122 ms: 1.01x slower                                                             |
| tornado_http               | 98.1 ms                                                | 99.0 ms: 1.01x slower                                                            |
| dask                       | 365 ms                                                 | 370 ms: 1.01x slower                                                             |
| docutils                   | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                           |
| bench_thread_pool          | 834 us                                                 | 848 us: 1.02x slower                                                             |
| sympy_expand               | 484 ms                                                 | 496 ms: 1.02x slower                                                             |
| create_gc_cycles           | 1.43 ms                                                | 1.47 ms: 1.03x slower                                                            |
| meteor_contest             | 109 ms                                                 | 112 ms: 1.03x slower                                                             |
| sqlglot_optimize           | 55.3 ms                                                | 57.1 ms: 1.03x slower                                                            |
| regex_effbot               | 3.51 ms                                                | 3.67 ms: 1.05x slower                                                            |
| nqueens                    | 87.9 ms                                                | 92.3 ms: 1.05x slower                                                            |
| xml_etree_process          | 56.9 ms                                                | 60.1 ms: 1.06x slower                                                            |
| regex_compile              | 141 ms                                                 | 149 ms: 1.06x slower                                                             |
| pprint_pformat             | 1.55 sec                                               | 1.65 sec: 1.06x slower                                                           |
| pprint_safe_repr           | 747 ms                                                 | 795 ms: 1.06x slower                                                             |
| crypto_pyaes               | 76.7 ms                                                | 81.7 ms: 1.06x slower                                                            |
| pickle                     | 11.0 us                                                | 11.7 us: 1.07x slower                                                            |
| pycparser                  | 1.19 sec                                               | 1.27 sec: 1.07x slower                                                           |
| 2to3                       | 264 ms                                                 | 284 ms: 1.07x slower                                                             |
| regex_dna                  | 205 ms                                                 | 220 ms: 1.08x slower                                                             |
| dulwich_log                | 64.6 ms                                                | 69.9 ms: 1.08x slower                                                            |
| chameleon                  | 6.70 ms                                                | 7.28 ms: 1.09x slower                                                            |
| fannkuch                   | 405 ms                                                 | 441 ms: 1.09x slower                                                             |
| xml_etree_generate         | 81.1 ms                                                | 88.3 ms: 1.09x slower                                                            |
| regex_v8                   | 22.9 ms                                                | 25.0 ms: 1.09x slower                                                            |
| tomli_loads                | 2.30 sec                                               | 2.55 sec: 1.11x slower                                                           |
| sqlite_synth               | 2.57 us                                                | 2.85 us: 1.11x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 79.9 ms: 1.13x slower                                                            |
| nbody                      | 96.0 ms                                                | 109 ms: 1.13x slower                                                             |
| float                      | 78.9 ms                                                | 90.0 ms: 1.14x slower                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.75 ms: 1.14x slower                                                            |
| pickle_list                | 4.59 us                                                | 5.26 us: 1.15x slower                                                            |
| unpack_sequence            | 43.5 ns                                                | 50.7 ns: 1.17x slower                                                            |
| pyflate                    | 434 ms                                                 | 509 ms: 1.17x slower                                                             |
| go                         | 149 ms                                                 | 175 ms: 1.18x slower                                                             |
| hexiom                     | 6.89 ms                                                | 8.11 ms: 1.18x slower                                                            |
| unpickle                   | 13.8 us                                                | 16.3 us: 1.18x slower                                                            |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| coverage                   | 78.8 ms                                                | 95.8 ms: 1.22x slower                                                            |
| async_generators           | 374 ms                                                 | 457 ms: 1.22x slower                                                             |
| mako                       | 10.7 ms                                                | 13.1 ms: 1.23x slower                                                            |
| spectral_norm              | 108 ms                                                 | 134 ms: 1.24x slower                                                             |
| scimark_fft                | 345 ms                                                 | 431 ms: 1.25x slower                                                             |
| telco                      | 6.86 ms                                                | 8.79 ms: 1.28x slower                                                            |
| python_startup_no_site     | 6.01 ms                                                | 8.80 ms: 1.46x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (8): pathlib, bench_mp_pool, pickle_dict, xml_etree_iterparse, sqlglot_normalize, scimark_lu, asyncio_websockets, json
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 89.85% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x