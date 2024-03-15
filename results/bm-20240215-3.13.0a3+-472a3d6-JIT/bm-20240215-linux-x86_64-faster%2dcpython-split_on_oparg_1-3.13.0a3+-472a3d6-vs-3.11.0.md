
# Results vs. 3.11.0

- fork: faster-cpython
- ref: split_on_oparg_1
- machine: linux-x86_64
- commit hash: 472a3d6
- commit date: 2024-02-15
- overall geometric mean: 1.04x faster \*
- HPT reliability: 93.85%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 277 ms: 1.05x slower                                                         |
| chameleon      | 6.70 ms                                                | 6.84 ms: 1.02x slower                                                        |
| docutils       | 2.66 sec                                               | 2.64 sec: 1.01x faster                                                       |
| tornado_http   | 98.1 ms                                                | 96.7 ms: 1.01x faster                                                        |
| Geometric mean | (ref)                                                  | 1.01x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 439 ms: 1.20x faster                                                         |
| async_tree_memoization     | 639 ms                                                 | 559 ms: 1.14x faster                                                         |
| async_tree_io              | 1.29 sec                                               | 1.16 sec: 1.11x faster                                                       |
| async_tree_none_tg         | 491 ms                                                 | 444 ms: 1.11x faster                                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.18 sec: 1.10x faster                                                       |
| async_tree_memoization_tg  | 626 ms                                                 | 571 ms: 1.10x faster                                                         |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 717 ms: 1.06x faster                                                         |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 706 ms: 1.06x faster                                                         |
| Geometric mean             | (ref)                                                  | 1.11x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                         |
| float          | 78.9 ms                                                | 83.0 ms: 1.05x slower                                                        |
| nbody          | 96.0 ms                                                | 101 ms: 1.06x slower                                                         |
| Geometric mean | (ref)                                                  | 1.02x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 138 ms: 1.02x faster                                                         |
| regex_effbot   | 3.51 ms                                                | 3.62 ms: 1.03x slower                                                        |
| regex_dna      | 205 ms                                                 | 219 ms: 1.07x slower                                                         |
| regex_v8       | 22.9 ms                                                | 24.6 ms: 1.07x slower                                                        |
| Geometric mean | (ref)                                                  | 1.04x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.28x faster                                                        |
| unpickle_pure_python | 242 us                                                 | 225 us: 1.07x faster                                                         |
| pickle_pure_python   | 320 us                                                 | 299 us: 1.07x faster                                                         |
| json_loads           | 29.2 us                                                | 27.6 us: 1.06x faster                                                        |
| tomli_loads          | 2.30 sec                                               | 2.18 sec: 1.06x faster                                                       |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                                         |
| pickle_dict          | 34.6 us                                                | 33.4 us: 1.04x faster                                                        |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                         |
| unpickle_list        | 5.21 us                                                | 5.16 us: 1.01x faster                                                        |
| xml_etree_process    | 56.9 ms                                                | 58.1 ms: 1.02x slower                                                        |
| pickle               | 11.0 us                                                | 11.3 us: 1.03x slower                                                        |
| xml_etree_generate   | 81.1 ms                                                | 85.2 ms: 1.05x slower                                                        |
| pickle_list          | 4.59 us                                                | 4.91 us: 1.07x slower                                                        |
| unpickle             | 13.8 us                                                | 15.1 us: 1.09x slower                                                        |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                        |
| python_startup_no_site | 6.01 ms                                                | 8.84 ms: 1.47x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 12.1 ms: 1.14x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.72x faster                                                         |
| generators                 | 74.9 ms                                                | 29.9 ms: 2.50x faster                                                        |
| asyncio_tcp                | 875 ms                                                 | 487 ms: 1.80x faster                                                         |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.73x faster                                                       |
| comprehensions             | 23.6 us                                                | 18.0 us: 1.31x faster                                                        |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.28x faster                                                        |
| richards_super             | 61.9 ms                                                | 51.3 ms: 1.21x faster                                                        |
| async_tree_none            | 528 ms                                                 | 439 ms: 1.20x faster                                                         |
| coroutines                 | 27.0 ms                                                | 22.8 ms: 1.19x faster                                                        |
| deltablue                  | 3.92 ms                                                | 3.31 ms: 1.18x faster                                                        |
| gc_traversal               | 4.01 ms                                                | 3.47 ms: 1.16x faster                                                        |
| async_tree_memoization     | 639 ms                                                 | 559 ms: 1.14x faster                                                         |
| sqlglot_parse              | 1.43 ms                                                | 1.29 ms: 1.11x faster                                                        |
| async_tree_io              | 1.29 sec                                               | 1.16 sec: 1.11x faster                                                       |
| async_tree_none_tg         | 491 ms                                                 | 444 ms: 1.11x faster                                                         |
| richards                   | 49.8 ms                                                | 45.2 ms: 1.10x faster                                                        |
| raytrace                   | 309 ms                                                 | 280 ms: 1.10x faster                                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.18 sec: 1.10x faster                                                       |
| async_tree_memoization_tg  | 626 ms                                                 | 571 ms: 1.10x faster                                                         |
| logging_silent             | 111 ns                                                 | 101 ns: 1.09x faster                                                         |
| logging_simple             | 6.22 us                                                | 5.71 us: 1.09x faster                                                        |
| sqlglot_transpile          | 1.75 ms                                                | 1.62 ms: 1.08x faster                                                        |
| unpickle_pure_python       | 242 us                                                 | 225 us: 1.07x faster                                                         |
| sympy_sum                  | 169 ms                                                 | 158 ms: 1.07x faster                                                         |
| mdp                        | 2.77 sec                                               | 2.59 sec: 1.07x faster                                                       |
| pickle_pure_python         | 320 us                                                 | 299 us: 1.07x faster                                                         |
| logging_format             | 6.81 us                                                | 6.39 us: 1.06x faster                                                        |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 717 ms: 1.06x faster                                                         |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 706 ms: 1.06x faster                                                         |
| sympy_str                  | 297 ms                                                 | 281 ms: 1.06x faster                                                         |
| json_loads                 | 29.2 us                                                | 27.6 us: 1.06x faster                                                        |
| tomli_loads                | 2.30 sec                                               | 2.18 sec: 1.06x faster                                                       |
| sympy_integrate            | 21.5 ms                                                | 20.4 ms: 1.05x faster                                                        |
| xml_etree_parse            | 164 ms                                                 | 156 ms: 1.05x faster                                                         |
| deepcopy_reduce            | 3.22 us                                                | 3.07 us: 1.05x faster                                                        |
| deepcopy_memo              | 40.2 us                                                | 38.3 us: 1.05x faster                                                        |
| deepcopy                   | 365 us                                                 | 349 us: 1.05x faster                                                         |
| sqlglot_normalize          | 113 ms                                                 | 109 ms: 1.04x faster                                                         |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                         |
| json                       | 5.24 ms                                                | 5.06 ms: 1.04x faster                                                        |
| pickle_dict                | 34.6 us                                                | 33.4 us: 1.04x faster                                                        |
| regex_compile              | 141 ms                                                 | 138 ms: 1.02x faster                                                         |
| scimark_lu                 | 116 ms                                                 | 114 ms: 1.02x faster                                                         |
| chaos                      | 71.9 ms                                                | 70.6 ms: 1.02x faster                                                        |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                                         |
| scimark_sor                | 121 ms                                                 | 119 ms: 1.02x faster                                                         |
| pathlib                    | 18.5 ms                                                | 18.3 ms: 1.01x faster                                                        |
| tornado_http               | 98.1 ms                                                | 96.7 ms: 1.01x faster                                                        |
| sympy_expand               | 484 ms                                                 | 478 ms: 1.01x faster                                                         |
| unpickle_list              | 5.21 us                                                | 5.16 us: 1.01x faster                                                        |
| docutils                   | 2.66 sec                                               | 2.64 sec: 1.01x faster                                                       |
| go                         | 149 ms                                                 | 148 ms: 1.01x faster                                                         |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                         |
| bench_thread_pool          | 834 us                                                 | 840 us: 1.01x slower                                                         |
| nqueens                    | 87.9 ms                                                | 89.1 ms: 1.01x slower                                                        |
| create_gc_cycles           | 1.43 ms                                                | 1.46 ms: 1.02x slower                                                        |
| xml_etree_process          | 56.9 ms                                                | 58.1 ms: 1.02x slower                                                        |
| chameleon                  | 6.70 ms                                                | 6.84 ms: 1.02x slower                                                        |
| crypto_pyaes               | 76.7 ms                                                | 78.5 ms: 1.02x slower                                                        |
| fannkuch                   | 405 ms                                                 | 417 ms: 1.03x slower                                                         |
| pickle                     | 11.0 us                                                | 11.3 us: 1.03x slower                                                        |
| regex_effbot               | 3.51 ms                                                | 3.62 ms: 1.03x slower                                                        |
| scimark_monte_carlo        | 70.7 ms                                                | 73.5 ms: 1.04x slower                                                        |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.27 ms: 1.05x slower                                                        |
| dulwich_log                | 64.6 ms                                                | 67.7 ms: 1.05x slower                                                        |
| pprint_pformat             | 1.55 sec                                               | 1.63 sec: 1.05x slower                                                       |
| 2to3                       | 264 ms                                                 | 277 ms: 1.05x slower                                                         |
| pprint_safe_repr           | 747 ms                                                 | 785 ms: 1.05x slower                                                         |
| xml_etree_generate         | 81.1 ms                                                | 85.2 ms: 1.05x slower                                                        |
| float                      | 78.9 ms                                                | 83.0 ms: 1.05x slower                                                        |
| nbody                      | 96.0 ms                                                | 101 ms: 1.06x slower                                                         |
| scimark_fft                | 345 ms                                                 | 367 ms: 1.06x slower                                                         |
| regex_dna                  | 205 ms                                                 | 219 ms: 1.07x slower                                                         |
| pickle_list                | 4.59 us                                                | 4.91 us: 1.07x slower                                                        |
| regex_v8                   | 22.9 ms                                                | 24.6 ms: 1.07x slower                                                        |
| unpickle                   | 13.8 us                                                | 15.1 us: 1.09x slower                                                        |
| sqlite_synth               | 2.57 us                                                | 2.83 us: 1.10x slower                                                        |
| hexiom                     | 6.89 ms                                                | 7.61 ms: 1.10x slower                                                        |
| mako                       | 10.7 ms                                                | 12.1 ms: 1.14x slower                                                        |
| pyflate                    | 434 ms                                                 | 497 ms: 1.15x slower                                                         |
| spectral_norm              | 108 ms                                                 | 126 ms: 1.17x slower                                                         |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                        |
| unpack_sequence            | 43.5 ns                                                | 52.0 ns: 1.20x slower                                                        |
| coverage                   | 78.8 ms                                                | 95.4 ms: 1.21x slower                                                        |
| async_generators           | 374 ms                                                 | 458 ms: 1.23x slower                                                         |
| telco                      | 6.86 ms                                                | 8.61 ms: 1.26x slower                                                        |
| mypy2                      | 686 ms                                                 | 863 ms: 1.26x slower                                                         |
| python_startup_no_site     | 6.01 ms                                                | 8.84 ms: 1.47x slower                                                        |
| Geometric mean             | (ref)                                                  | 1.04x faster                                                                 |

Benchmark hidden because not significant (5): pycparser, bench_mp_pool, sqlglot_optimize, meteor_contest, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 93.85% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x