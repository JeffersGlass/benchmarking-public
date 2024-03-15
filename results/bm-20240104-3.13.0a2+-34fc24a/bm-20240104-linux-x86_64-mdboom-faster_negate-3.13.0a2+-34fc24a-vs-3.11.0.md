
# Results vs. 3.11.0

- fork: mdboom
- ref: faster_negate
- machine: linux-x86_64
- commit hash: 34fc24a
- commit date: 2024-01-04
- overall geometric mean: 1.07x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 265 ms: 1.00x slower                                            |
| chameleon      | 6.70 ms                                                | 6.87 ms: 1.03x slower                                           |
| docutils       | 2.66 sec                                               | 2.59 sec: 1.03x faster                                          |
| tornado_http   | 98.1 ms                                                | 94.2 ms: 1.04x faster                                           |
| Geometric mean | (ref)                                                  | 1.01x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 434 ms: 1.22x faster                                            |
| async_tree_memoization     | 639 ms                                                 | 558 ms: 1.14x faster                                            |
| async_tree_none_tg         | 491 ms                                                 | 441 ms: 1.11x faster                                            |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                          |
| async_tree_memoization_tg  | 626 ms                                                 | 574 ms: 1.09x faster                                            |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.08x faster                                          |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 703 ms: 1.07x faster                                            |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 720 ms: 1.06x faster                                            |
| Geometric mean             | (ref)                                                  | 1.11x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 90.1 ms: 1.07x faster                                           |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                            |
| float          | 78.9 ms                                                | 80.3 ms: 1.02x slower                                           |
| Geometric mean | (ref)                                                  | 1.03x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 130 ms: 1.08x faster                                            |
| regex_effbot   | 3.51 ms                                                | 3.64 ms: 1.04x slower                                           |
| regex_v8       | 22.9 ms                                                | 25.0 ms: 1.09x slower                                           |
| regex_dna      | 205 ms                                                 | 225 ms: 1.10x slower                                            |
| Geometric mean | (ref)                                                  | 1.04x slower                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.26x faster                                           |
| unpickle_pure_python | 242 us                                                 | 219 us: 1.10x faster                                            |
| tomli_loads          | 2.30 sec                                               | 2.18 sec: 1.06x faster                                          |
| pickle_pure_python   | 320 us                                                 | 305 us: 1.05x faster                                            |
| json_loads           | 29.2 us                                                | 28.3 us: 1.03x faster                                           |
| xml_etree_iterparse  | 108 ms                                                 | 105 ms: 1.03x faster                                            |
| xml_etree_parse      | 164 ms                                                 | 160 ms: 1.02x faster                                            |
| unpickle_list        | 5.21 us                                                | 5.10 us: 1.02x faster                                           |
| pickle_dict          | 34.6 us                                                | 34.2 us: 1.01x faster                                           |
| xml_etree_process    | 56.9 ms                                                | 58.9 ms: 1.04x slower                                           |
| pickle               | 11.0 us                                                | 11.4 us: 1.04x slower                                           |
| xml_etree_generate   | 81.1 ms                                                | 85.8 ms: 1.06x slower                                           |
| pickle_list          | 4.59 us                                                | 4.90 us: 1.07x slower                                           |
| unpickle             | 13.8 us                                                | 15.7 us: 1.14x slower                                           |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                           |
| python_startup_no_site | 6.01 ms                                                | 8.73 ms: 1.45x slower                                           |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.2 ms: 1.05x slower                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 109 us: 4.78x faster                                            |
| generators                 | 74.9 ms                                                | 29.5 ms: 2.54x faster                                           |
| asyncio_tcp                | 875 ms                                                 | 484 ms: 1.81x faster                                            |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.78 sec: 1.75x faster                                          |
| comprehensions             | 23.6 us                                                | 16.4 us: 1.44x faster                                           |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.26x faster                                           |
| coroutines                 | 27.0 ms                                                | 22.1 ms: 1.23x faster                                           |
| async_tree_none            | 528 ms                                                 | 434 ms: 1.22x faster                                            |
| deltablue                  | 3.92 ms                                                | 3.25 ms: 1.21x faster                                           |
| chaos                      | 71.9 ms                                                | 60.1 ms: 1.20x faster                                           |
| raytrace                   | 309 ms                                                 | 261 ms: 1.18x faster                                            |
| richards_super             | 61.9 ms                                                | 53.7 ms: 1.15x faster                                           |
| sqlglot_parse              | 1.43 ms                                                | 1.24 ms: 1.15x faster                                           |
| async_tree_memoization     | 639 ms                                                 | 558 ms: 1.14x faster                                            |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                            |
| sqlglot_transpile          | 1.75 ms                                                | 1.56 ms: 1.12x faster                                           |
| logging_simple             | 6.22 us                                                | 5.58 us: 1.12x faster                                           |
| async_tree_none_tg         | 491 ms                                                 | 441 ms: 1.11x faster                                            |
| sympy_str                  | 297 ms                                                 | 268 ms: 1.11x faster                                            |
| unpickle_pure_python       | 242 us                                                 | 219 us: 1.10x faster                                            |
| logging_format             | 6.81 us                                                | 6.19 us: 1.10x faster                                           |
| sympy_integrate            | 21.5 ms                                                | 19.5 ms: 1.10x faster                                           |
| hexiom                     | 6.89 ms                                                | 6.29 ms: 1.10x faster                                           |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                          |
| async_tree_memoization_tg  | 626 ms                                                 | 574 ms: 1.09x faster                                            |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.08x faster                                          |
| gc_traversal               | 4.01 ms                                                | 3.70 ms: 1.08x faster                                           |
| regex_compile              | 141 ms                                                 | 130 ms: 1.08x faster                                            |
| mdp                        | 2.77 sec                                               | 2.57 sec: 1.08x faster                                          |
| logging_silent             | 111 ns                                                 | 103 ns: 1.07x faster                                            |
| crypto_pyaes               | 76.7 ms                                                | 71.8 ms: 1.07x faster                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 703 ms: 1.07x faster                                            |
| nbody                      | 96.0 ms                                                | 90.1 ms: 1.07x faster                                           |
| sqlglot_normalize          | 113 ms                                                 | 106 ms: 1.06x faster                                            |
| sympy_expand               | 484 ms                                                 | 457 ms: 1.06x faster                                            |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 720 ms: 1.06x faster                                            |
| tomli_loads                | 2.30 sec                                               | 2.18 sec: 1.06x faster                                          |
| deepcopy                   | 365 us                                                 | 346 us: 1.06x faster                                            |
| go                         | 149 ms                                                 | 141 ms: 1.06x faster                                            |
| richards                   | 49.8 ms                                                | 47.2 ms: 1.05x faster                                           |
| pickle_pure_python         | 320 us                                                 | 305 us: 1.05x faster                                            |
| nqueens                    | 87.9 ms                                                | 83.9 ms: 1.05x faster                                           |
| deepcopy_reduce            | 3.22 us                                                | 3.08 us: 1.04x faster                                           |
| deepcopy_memo              | 40.2 us                                                | 38.6 us: 1.04x faster                                           |
| tornado_http               | 98.1 ms                                                | 94.2 ms: 1.04x faster                                           |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                            |
| pprint_pformat             | 1.55 sec                                               | 1.50 sec: 1.04x faster                                          |
| scimark_lu                 | 116 ms                                                 | 112 ms: 1.04x faster                                            |
| sqlglot_optimize           | 55.3 ms                                                | 53.5 ms: 1.03x faster                                           |
| scimark_monte_carlo        | 70.7 ms                                                | 68.4 ms: 1.03x faster                                           |
| json_loads                 | 29.2 us                                                | 28.3 us: 1.03x faster                                           |
| xml_etree_iterparse        | 108 ms                                                 | 105 ms: 1.03x faster                                            |
| docutils                   | 2.66 sec                                               | 2.59 sec: 1.03x faster                                          |
| xml_etree_parse            | 164 ms                                                 | 160 ms: 1.02x faster                                            |
| unpickle_list              | 5.21 us                                                | 5.10 us: 1.02x faster                                           |
| meteor_contest             | 109 ms                                                 | 107 ms: 1.02x faster                                            |
| pathlib                    | 18.5 ms                                                | 18.2 ms: 1.02x faster                                           |
| pycparser                  | 1.19 sec                                               | 1.17 sec: 1.01x faster                                          |
| pprint_safe_repr           | 747 ms                                                 | 737 ms: 1.01x faster                                            |
| dask                       | 365 ms                                                 | 360 ms: 1.01x faster                                            |
| pickle_dict                | 34.6 us                                                | 34.2 us: 1.01x faster                                           |
| bench_thread_pool          | 834 us                                                 | 830 us: 1.01x faster                                            |
| fannkuch                   | 405 ms                                                 | 403 ms: 1.00x faster                                            |
| 2to3                       | 264 ms                                                 | 265 ms: 1.00x slower                                            |
| dulwich_log                | 64.6 ms                                                | 65.1 ms: 1.01x slower                                           |
| unpack_sequence            | 43.5 ns                                                | 44.1 ns: 1.01x slower                                           |
| float                      | 78.9 ms                                                | 80.3 ms: 1.02x slower                                           |
| chameleon                  | 6.70 ms                                                | 6.87 ms: 1.03x slower                                           |
| create_gc_cycles           | 1.43 ms                                                | 1.48 ms: 1.03x slower                                           |
| xml_etree_process          | 56.9 ms                                                | 58.9 ms: 1.04x slower                                           |
| pickle                     | 11.0 us                                                | 11.4 us: 1.04x slower                                           |
| regex_effbot               | 3.51 ms                                                | 3.64 ms: 1.04x slower                                           |
| pyflate                    | 434 ms                                                 | 456 ms: 1.05x slower                                            |
| scimark_fft                | 345 ms                                                 | 364 ms: 1.05x slower                                            |
| mako                       | 10.7 ms                                                | 11.2 ms: 1.05x slower                                           |
| xml_etree_generate         | 81.1 ms                                                | 85.8 ms: 1.06x slower                                           |
| spectral_norm              | 108 ms                                                 | 115 ms: 1.07x slower                                            |
| pickle_list                | 4.59 us                                                | 4.90 us: 1.07x slower                                           |
| scimark_sor                | 121 ms                                                 | 130 ms: 1.07x slower                                            |
| regex_v8                   | 22.9 ms                                                | 25.0 ms: 1.09x slower                                           |
| regex_dna                  | 205 ms                                                 | 225 ms: 1.10x slower                                            |
| sqlite_synth               | 2.57 us                                                | 2.86 us: 1.11x slower                                           |
| unpickle                   | 13.8 us                                                | 15.7 us: 1.14x slower                                           |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                           |
| async_generators           | 374 ms                                                 | 445 ms: 1.19x slower                                            |
| mypy2                      | 686 ms                                                 | 840 ms: 1.23x slower                                            |
| telco                      | 6.86 ms                                                | 8.42 ms: 1.23x slower                                           |
| coverage                   | 78.8 ms                                                | 97.0 ms: 1.23x slower                                           |
| python_startup_no_site     | 6.01 ms                                                | 8.73 ms: 1.45x slower                                           |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                    |

Benchmark hidden because not significant (4): scimark_sparse_mat_mult, bench_mp_pool, asyncio_websockets, json
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.98x