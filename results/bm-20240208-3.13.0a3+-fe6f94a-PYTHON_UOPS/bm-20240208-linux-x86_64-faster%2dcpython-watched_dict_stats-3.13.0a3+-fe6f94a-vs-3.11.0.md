
# Results vs. 3.11.0

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: fe6f94a
- commit date: 2024-02-08
- overall geometric mean: 1.03x slower \*
- HPT reliability: 99.78%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 288 ms: 1.09x slower                                                           |
| chameleon      | 6.70 ms                                                | 7.37 ms: 1.10x slower                                                          |
| docutils       | 2.66 sec                                               | 2.71 sec: 1.02x slower                                                         |
| tornado_http   | 98.1 ms                                                | 99.4 ms: 1.01x slower                                                          |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 457 ms: 1.15x faster                                                           |
| async_tree_memoization     | 639 ms                                                 | 582 ms: 1.10x faster                                                           |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                         |
| async_tree_none_tg         | 491 ms                                                 | 462 ms: 1.06x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 598 ms: 1.05x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 735 ms: 1.04x faster                                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 727 ms: 1.03x faster                                                           |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                           |
| float          | 78.9 ms                                                | 105 ms: 1.34x slower                                                           |
| nbody          | 96.0 ms                                                | 141 ms: 1.46x slower                                                           |
| Geometric mean | (ref)                                                  | 1.24x slower                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.70 ms: 1.05x slower                                                          |
| regex_v8       | 22.9 ms                                                | 24.4 ms: 1.07x slower                                                          |
| regex_dna      | 205 ms                                                 | 225 ms: 1.10x slower                                                           |
| regex_compile  | 141 ms                                                 | 157 ms: 1.11x slower                                                           |
| Geometric mean | (ref)                                                  | 1.08x slower                                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                          |
| pickle_pure_python   | 320 us                                                 | 301 us: 1.06x faster                                                           |
| json_loads           | 29.2 us                                                | 27.8 us: 1.05x faster                                                          |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                           |
| unpickle_list        | 5.21 us                                                | 5.17 us: 1.01x faster                                                          |
| unpickle_pure_python | 242 us                                                 | 240 us: 1.01x faster                                                           |
| pickle_dict          | 34.6 us                                                | 35.3 us: 1.02x slower                                                          |
| xml_etree_iterparse  | 108 ms                                                 | 115 ms: 1.06x slower                                                           |
| pickle               | 11.0 us                                                | 11.9 us: 1.08x slower                                                          |
| xml_etree_process    | 56.9 ms                                                | 61.8 ms: 1.09x slower                                                          |
| unpickle             | 13.8 us                                                | 15.2 us: 1.10x slower                                                          |
| xml_etree_generate   | 81.1 ms                                                | 91.3 ms: 1.13x slower                                                          |
| pickle_list          | 4.59 us                                                | 5.24 us: 1.14x slower                                                          |
| tomli_loads          | 2.30 sec                                               | 2.84 sec: 1.23x slower                                                         |
| Geometric mean       | (ref)                                                  | 1.03x slower                                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                          |
| python_startup_no_site | 6.01 ms                                                | 8.81 ms: 1.46x slower                                                          |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 15.4 ms: 1.45x slower                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 119 us: 4.38x faster                                                           |
| generators                 | 74.9 ms                                                | 29.6 ms: 2.53x faster                                                          |
| asyncio_tcp                | 875 ms                                                 | 490 ms: 1.79x faster                                                           |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.81 sec: 1.72x faster                                                         |
| json_dumps                 | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                          |
| coroutines                 | 27.0 ms                                                | 22.9 ms: 1.18x faster                                                          |
| async_tree_none            | 528 ms                                                 | 457 ms: 1.15x faster                                                           |
| async_tree_memoization     | 639 ms                                                 | 582 ms: 1.10x faster                                                           |
| richards_super             | 61.9 ms                                                | 56.8 ms: 1.09x faster                                                          |
| gc_traversal               | 4.01 ms                                                | 3.70 ms: 1.08x faster                                                          |
| deltablue                  | 3.92 ms                                                | 3.63 ms: 1.08x faster                                                          |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                         |
| async_tree_none_tg         | 491 ms                                                 | 462 ms: 1.06x faster                                                           |
| pickle_pure_python         | 320 us                                                 | 301 us: 1.06x faster                                                           |
| json_loads                 | 29.2 us                                                | 27.8 us: 1.05x faster                                                          |
| sqlglot_parse              | 1.43 ms                                                | 1.37 ms: 1.05x faster                                                          |
| logging_silent             | 111 ns                                                 | 106 ns: 1.05x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 598 ms: 1.05x faster                                                           |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 735 ms: 1.04x faster                                                           |
| deepcopy_reduce            | 3.22 us                                                | 3.12 us: 1.03x faster                                                          |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 727 ms: 1.03x faster                                                           |
| sqlglot_transpile          | 1.75 ms                                                | 1.70 ms: 1.03x faster                                                          |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                           |
| deepcopy                   | 365 us                                                 | 356 us: 1.02x faster                                                           |
| sympy_sum                  | 169 ms                                                 | 165 ms: 1.02x faster                                                           |
| logging_simple             | 6.22 us                                                | 6.10 us: 1.02x faster                                                          |
| json                       | 5.24 ms                                                | 5.15 ms: 1.02x faster                                                          |
| unpickle_list              | 5.21 us                                                | 5.17 us: 1.01x faster                                                          |
| unpickle_pure_python       | 242 us                                                 | 240 us: 1.01x faster                                                           |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                           |
| richards                   | 49.8 ms                                                | 50.2 ms: 1.01x slower                                                          |
| pathlib                    | 18.5 ms                                                | 18.7 ms: 1.01x slower                                                          |
| raytrace                   | 309 ms                                                 | 312 ms: 1.01x slower                                                           |
| comprehensions             | 23.6 us                                                | 23.9 us: 1.01x slower                                                          |
| sympy_integrate            | 21.5 ms                                                | 21.7 ms: 1.01x slower                                                          |
| tornado_http               | 98.1 ms                                                | 99.4 ms: 1.01x slower                                                          |
| docutils                   | 2.66 sec                                               | 2.71 sec: 1.02x slower                                                         |
| mdp                        | 2.77 sec                                               | 2.83 sec: 1.02x slower                                                         |
| logging_format             | 6.81 us                                                | 6.94 us: 1.02x slower                                                          |
| sympy_expand               | 484 ms                                                 | 495 ms: 1.02x slower                                                           |
| pickle_dict                | 34.6 us                                                | 35.3 us: 1.02x slower                                                          |
| scimark_sor                | 121 ms                                                 | 124 ms: 1.02x slower                                                           |
| bench_thread_pool          | 834 us                                                 | 855 us: 1.02x slower                                                           |
| deepcopy_memo              | 40.2 us                                                | 41.2 us: 1.02x slower                                                          |
| scimark_lu                 | 116 ms                                                 | 119 ms: 1.03x slower                                                           |
| create_gc_cycles           | 1.43 ms                                                | 1.47 ms: 1.03x slower                                                          |
| sqlglot_normalize          | 113 ms                                                 | 117 ms: 1.03x slower                                                           |
| pycparser                  | 1.19 sec                                               | 1.23 sec: 1.04x slower                                                         |
| regex_effbot               | 3.51 ms                                                | 3.70 ms: 1.05x slower                                                          |
| xml_etree_iterparse        | 108 ms                                                 | 115 ms: 1.06x slower                                                           |
| regex_v8                   | 22.9 ms                                                | 24.4 ms: 1.07x slower                                                          |
| sqlglot_optimize           | 55.3 ms                                                | 59.0 ms: 1.07x slower                                                          |
| dulwich_log                | 64.6 ms                                                | 69.3 ms: 1.07x slower                                                          |
| pickle                     | 11.0 us                                                | 11.9 us: 1.08x slower                                                          |
| meteor_contest             | 109 ms                                                 | 118 ms: 1.08x slower                                                           |
| xml_etree_process          | 56.9 ms                                                | 61.8 ms: 1.09x slower                                                          |
| 2to3                       | 264 ms                                                 | 288 ms: 1.09x slower                                                           |
| regex_dna                  | 205 ms                                                 | 225 ms: 1.10x slower                                                           |
| chameleon                  | 6.70 ms                                                | 7.37 ms: 1.10x slower                                                          |
| unpickle                   | 13.8 us                                                | 15.2 us: 1.10x slower                                                          |
| chaos                      | 71.9 ms                                                | 79.8 ms: 1.11x slower                                                          |
| regex_compile              | 141 ms                                                 | 157 ms: 1.11x slower                                                           |
| pprint_safe_repr           | 747 ms                                                 | 834 ms: 1.12x slower                                                           |
| pprint_pformat             | 1.55 sec                                               | 1.75 sec: 1.12x slower                                                         |
| sqlite_synth               | 2.57 us                                                | 2.90 us: 1.13x slower                                                          |
| xml_etree_generate         | 81.1 ms                                                | 91.3 ms: 1.13x slower                                                          |
| pickle_list                | 4.59 us                                                | 5.24 us: 1.14x slower                                                          |
| nqueens                    | 87.9 ms                                                | 104 ms: 1.19x slower                                                           |
| go                         | 149 ms                                                 | 177 ms: 1.19x slower                                                           |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                          |
| coverage                   | 78.8 ms                                                | 94.7 ms: 1.20x slower                                                          |
| fannkuch                   | 405 ms                                                 | 490 ms: 1.21x slower                                                           |
| async_generators           | 374 ms                                                 | 456 ms: 1.22x slower                                                           |
| crypto_pyaes               | 76.7 ms                                                | 93.8 ms: 1.22x slower                                                          |
| tomli_loads                | 2.30 sec                                               | 2.84 sec: 1.23x slower                                                         |
| unpack_sequence            | 43.5 ns                                                | 54.6 ns: 1.26x slower                                                          |
| scimark_monte_carlo        | 70.7 ms                                                | 89.8 ms: 1.27x slower                                                          |
| mypy2                      | 686 ms                                                 | 873 ms: 1.27x slower                                                           |
| telco                      | 6.86 ms                                                | 8.95 ms: 1.30x slower                                                          |
| pyflate                    | 434 ms                                                 | 573 ms: 1.32x slower                                                           |
| float                      | 78.9 ms                                                | 105 ms: 1.34x slower                                                           |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.74 ms: 1.34x slower                                                          |
| hexiom                     | 6.89 ms                                                | 9.60 ms: 1.39x slower                                                          |
| scimark_fft                | 345 ms                                                 | 496 ms: 1.44x slower                                                           |
| mako                       | 10.7 ms                                                | 15.4 ms: 1.45x slower                                                          |
| nbody                      | 96.0 ms                                                | 141 ms: 1.46x slower                                                           |
| python_startup_no_site     | 6.01 ms                                                | 8.81 ms: 1.46x slower                                                          |
| spectral_norm              | 108 ms                                                 | 167 ms: 1.54x slower                                                           |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                                   |

Benchmark hidden because not significant (3): bench_mp_pool, sympy_str, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.78% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x