
# Results vs. 3.11.0

- fork: faster-cpython
- ref: globals_to_constants
- machine: linux-x86_64
- commit hash: 35a92cc
- commit date: 2024-01-18
- overall geometric mean: 1.01x faster
- HPT reliability: 90.59%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 281 ms: 1.06x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.22 ms: 1.08x slower                                                            |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                           |
| tornado_http   | 98.1 ms                                                | 101 ms: 1.03x slower                                                             |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 449 ms: 1.18x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 577 ms: 1.11x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 457 ms: 1.07x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 584 ms: 1.07x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 719 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 732 ms: 1.04x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| float          | 78.9 ms                                                | 90.0 ms: 1.14x slower                                                            |
| nbody          | 96.0 ms                                                | 111 ms: 1.15x slower                                                             |
| Geometric mean | (ref)                                                  | 1.08x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.52 ms: 1.00x slower                                                            |
| regex_compile  | 141 ms                                                 | 149 ms: 1.06x slower                                                             |
| regex_dna      | 205 ms                                                 | 219 ms: 1.07x slower                                                             |
| regex_v8       | 22.9 ms                                                | 25.0 ms: 1.09x slower                                                            |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.25x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 298 us: 1.07x faster                                                             |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.05x faster                                                             |
| unpickle_pure_python | 242 us                                                 | 231 us: 1.05x faster                                                             |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                                            |
| pickle_dict          | 34.6 us                                                | 35.1 us: 1.02x slower                                                            |
| pickle               | 11.0 us                                                | 11.4 us: 1.04x slower                                                            |
| unpickle_list        | 5.21 us                                                | 5.45 us: 1.04x slower                                                            |
| pickle_list          | 4.59 us                                                | 4.85 us: 1.06x slower                                                            |
| xml_etree_process    | 56.9 ms                                                | 60.4 ms: 1.06x slower                                                            |
| unpickle             | 13.8 us                                                | 14.8 us: 1.07x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 88.0 ms: 1.09x slower                                                            |
| tomli_loads          | 2.30 sec                                               | 2.55 sec: 1.11x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.72 ms: 1.45x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.2 ms: 1.24x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 114 us: 4.54x faster                                                             |
| generators                 | 74.9 ms                                                | 29.7 ms: 2.52x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 482 ms: 1.82x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.73x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.6 ms: 1.25x faster                                                            |
| coroutines                 | 27.0 ms                                                | 22.6 ms: 1.20x faster                                                            |
| async_tree_none            | 528 ms                                                 | 449 ms: 1.18x faster                                                             |
| comprehensions             | 23.6 us                                                | 20.6 us: 1.14x faster                                                            |
| richards_super             | 61.9 ms                                                | 55.2 ms: 1.12x faster                                                            |
| deltablue                  | 3.92 ms                                                | 3.51 ms: 1.12x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 577 ms: 1.11x faster                                                             |
| gc_traversal               | 4.01 ms                                                | 3.70 ms: 1.08x faster                                                            |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                           |
| pickle_pure_python         | 320 us                                                 | 298 us: 1.07x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 457 ms: 1.07x faster                                                             |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.07x faster                                                            |
| async_tree_memoization_tg  | 626 ms                                                 | 584 ms: 1.07x faster                                                             |
| unpack_sequence            | 43.5 ns                                                | 40.7 ns: 1.07x faster                                                            |
| logging_silent             | 111 ns                                                 | 105 ns: 1.06x faster                                                             |
| sqlglot_transpile          | 1.75 ms                                                | 1.67 ms: 1.05x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 161 ms: 1.05x faster                                                             |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.05x faster                                                             |
| unpickle_pure_python       | 242 us                                                 | 231 us: 1.05x faster                                                             |
| raytrace                   | 309 ms                                                 | 296 ms: 1.04x faster                                                             |
| mdp                        | 2.77 sec                                               | 2.66 sec: 1.04x faster                                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 719 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 732 ms: 1.04x faster                                                             |
| json_loads                 | 29.2 us                                                | 28.1 us: 1.04x faster                                                            |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| logging_simple             | 6.22 us                                                | 6.10 us: 1.02x faster                                                            |
| json                       | 5.24 ms                                                | 5.14 ms: 1.02x faster                                                            |
| deepcopy                   | 365 us                                                 | 358 us: 1.02x faster                                                             |
| richards                   | 49.8 ms                                                | 48.8 ms: 1.02x faster                                                            |
| sympy_integrate            | 21.5 ms                                                | 21.1 ms: 1.02x faster                                                            |
| logging_format             | 6.81 us                                                | 6.76 us: 1.01x faster                                                            |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                             |
| regex_effbot               | 3.51 ms                                                | 3.52 ms: 1.00x slower                                                            |
| sympy_expand               | 484 ms                                                 | 488 ms: 1.01x slower                                                             |
| bench_thread_pool          | 834 us                                                 | 841 us: 1.01x slower                                                             |
| dask                       | 365 ms                                                 | 369 ms: 1.01x slower                                                             |
| docutils                   | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                           |
| pickle_dict                | 34.6 us                                                | 35.1 us: 1.02x slower                                                            |
| sqlglot_normalize          | 113 ms                                                 | 115 ms: 1.02x slower                                                             |
| sympy_str                  | 297 ms                                                 | 303 ms: 1.02x slower                                                             |
| scimark_lu                 | 116 ms                                                 | 119 ms: 1.02x slower                                                             |
| scimark_sor                | 121 ms                                                 | 124 ms: 1.02x slower                                                             |
| tornado_http               | 98.1 ms                                                | 101 ms: 1.03x slower                                                             |
| pickle                     | 11.0 us                                                | 11.4 us: 1.04x slower                                                            |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                                            |
| meteor_contest             | 109 ms                                                 | 114 ms: 1.04x slower                                                             |
| unpickle_list              | 5.21 us                                                | 5.45 us: 1.04x slower                                                            |
| sqlglot_optimize           | 55.3 ms                                                | 57.9 ms: 1.05x slower                                                            |
| pycparser                  | 1.19 sec                                               | 1.25 sec: 1.05x slower                                                           |
| regex_compile              | 141 ms                                                 | 149 ms: 1.06x slower                                                             |
| pickle_list                | 4.59 us                                                | 4.85 us: 1.06x slower                                                            |
| xml_etree_process          | 56.9 ms                                                | 60.4 ms: 1.06x slower                                                            |
| nqueens                    | 87.9 ms                                                | 93.4 ms: 1.06x slower                                                            |
| 2to3                       | 264 ms                                                 | 281 ms: 1.06x slower                                                             |
| pprint_safe_repr           | 747 ms                                                 | 794 ms: 1.06x slower                                                             |
| crypto_pyaes               | 76.7 ms                                                | 81.6 ms: 1.06x slower                                                            |
| pprint_pformat             | 1.55 sec                                               | 1.66 sec: 1.07x slower                                                           |
| regex_dna                  | 205 ms                                                 | 219 ms: 1.07x slower                                                             |
| unpickle                   | 13.8 us                                                | 14.8 us: 1.07x slower                                                            |
| dulwich_log                | 64.6 ms                                                | 69.3 ms: 1.07x slower                                                            |
| chameleon                  | 6.70 ms                                                | 7.22 ms: 1.08x slower                                                            |
| fannkuch                   | 405 ms                                                 | 439 ms: 1.08x slower                                                             |
| xml_etree_generate         | 81.1 ms                                                | 88.0 ms: 1.09x slower                                                            |
| regex_v8                   | 22.9 ms                                                | 25.0 ms: 1.09x slower                                                            |
| tomli_loads                | 2.30 sec                                               | 2.55 sec: 1.11x slower                                                           |
| scimark_monte_carlo        | 70.7 ms                                                | 78.4 ms: 1.11x slower                                                            |
| sqlite_synth               | 2.57 us                                                | 2.86 us: 1.11x slower                                                            |
| float                      | 78.9 ms                                                | 90.0 ms: 1.14x slower                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.80 ms: 1.15x slower                                                            |
| nbody                      | 96.0 ms                                                | 111 ms: 1.15x slower                                                             |
| hexiom                     | 6.89 ms                                                | 8.04 ms: 1.17x slower                                                            |
| go                         | 149 ms                                                 | 174 ms: 1.17x slower                                                             |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                            |
| pyflate                    | 434 ms                                                 | 521 ms: 1.20x slower                                                             |
| async_generators           | 374 ms                                                 | 451 ms: 1.21x slower                                                             |
| coverage                   | 78.8 ms                                                | 95.7 ms: 1.21x slower                                                            |
| mako                       | 10.7 ms                                                | 13.2 ms: 1.24x slower                                                            |
| telco                      | 6.86 ms                                                | 8.57 ms: 1.25x slower                                                            |
| mypy2                      | 686 ms                                                 | 863 ms: 1.26x slower                                                             |
| scimark_fft                | 345 ms                                                 | 436 ms: 1.26x slower                                                             |
| spectral_norm              | 108 ms                                                 | 140 ms: 1.29x slower                                                             |
| python_startup_no_site     | 6.01 ms                                                | 8.72 ms: 1.45x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (6): deepcopy_memo, chaos, bench_mp_pool, pathlib, deepcopy_reduce, xml_etree_iterparse
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 90.59% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x