
# Results vs. 3.11.0

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: 1054202
- commit date: 2024-02-09
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 264 ms: 1.00x faster                                                           |
| chameleon      | 6.70 ms                                                | 6.92 ms: 1.03x slower                                                          |
| docutils       | 2.66 sec                                               | 2.59 sec: 1.03x faster                                                         |
| tornado_http   | 98.1 ms                                                | 94.4 ms: 1.04x faster                                                          |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 433 ms: 1.22x faster                                                           |
| async_tree_memoization     | 639 ms                                                 | 560 ms: 1.14x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 442 ms: 1.11x faster                                                           |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                         |
| async_tree_memoization_tg  | 626 ms                                                 | 570 ms: 1.10x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                         |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 702 ms: 1.07x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 718 ms: 1.06x faster                                                           |
| Geometric mean             | (ref)                                                  | 1.11x faster                                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 90.3 ms: 1.06x faster                                                          |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                           |
| float          | 78.9 ms                                                | 80.5 ms: 1.02x slower                                                          |
| Geometric mean | (ref)                                                  | 1.03x faster                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 130 ms: 1.09x faster                                                           |
| regex_effbot   | 3.51 ms                                                | 3.64 ms: 1.04x slower                                                          |
| regex_dna      | 205 ms                                                 | 220 ms: 1.07x slower                                                           |
| regex_v8       | 22.9 ms                                                | 25.0 ms: 1.09x slower                                                          |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                          |
| unpickle_pure_python | 242 us                                                 | 212 us: 1.14x faster                                                           |
| tomli_loads          | 2.30 sec                                               | 2.12 sec: 1.09x faster                                                         |
| pickle_pure_python   | 320 us                                                 | 296 us: 1.08x faster                                                           |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                                           |
| pickle_dict          | 34.6 us                                                | 33.0 us: 1.05x faster                                                          |
| unpickle_list        | 5.21 us                                                | 5.02 us: 1.04x faster                                                          |
| json_loads           | 29.2 us                                                | 28.2 us: 1.04x faster                                                          |
| xml_etree_iterparse  | 108 ms                                                 | 105 ms: 1.03x faster                                                           |
| xml_etree_process    | 56.9 ms                                                | 58.3 ms: 1.02x slower                                                          |
| pickle               | 11.0 us                                                | 11.4 us: 1.04x slower                                                          |
| xml_etree_generate   | 81.1 ms                                                | 85.8 ms: 1.06x slower                                                          |
| pickle_list          | 4.59 us                                                | 5.04 us: 1.10x slower                                                          |
| unpickle             | 13.8 us                                                | 15.4 us: 1.11x slower                                                          |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                          |
| python_startup_no_site | 6.01 ms                                                | 8.77 ms: 1.46x slower                                                          |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.2 ms: 1.05x slower                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 109 us: 4.77x faster                                                           |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.55x faster                                                          |
| asyncio_tcp                | 875 ms                                                 | 485 ms: 1.81x faster                                                           |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.78 sec: 1.74x faster                                                         |
| comprehensions             | 23.6 us                                                | 16.1 us: 1.47x faster                                                          |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                          |
| chaos                      | 71.9 ms                                                | 58.2 ms: 1.23x faster                                                          |
| coroutines                 | 27.0 ms                                                | 22.0 ms: 1.23x faster                                                          |
| async_tree_none            | 528 ms                                                 | 433 ms: 1.22x faster                                                           |
| deltablue                  | 3.92 ms                                                | 3.22 ms: 1.22x faster                                                          |
| raytrace                   | 309 ms                                                 | 258 ms: 1.20x faster                                                           |
| richards_super             | 61.9 ms                                                | 52.7 ms: 1.17x faster                                                          |
| hexiom                     | 6.89 ms                                                | 6.01 ms: 1.15x faster                                                          |
| async_tree_memoization     | 639 ms                                                 | 560 ms: 1.14x faster                                                           |
| unpickle_pure_python       | 242 us                                                 | 212 us: 1.14x faster                                                           |
| sqlglot_parse              | 1.43 ms                                                | 1.26 ms: 1.14x faster                                                          |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                                           |
| logging_silent             | 111 ns                                                 | 98.5 ns: 1.13x faster                                                          |
| logging_simple             | 6.22 us                                                | 5.58 us: 1.11x faster                                                          |
| sqlglot_transpile          | 1.75 ms                                                | 1.57 ms: 1.11x faster                                                          |
| async_tree_none_tg         | 491 ms                                                 | 442 ms: 1.11x faster                                                           |
| logging_format             | 6.81 us                                                | 6.15 us: 1.11x faster                                                          |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                         |
| async_tree_memoization_tg  | 626 ms                                                 | 570 ms: 1.10x faster                                                           |
| sympy_str                  | 297 ms                                                 | 271 ms: 1.10x faster                                                           |
| mdp                        | 2.77 sec                                               | 2.53 sec: 1.10x faster                                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                         |
| sympy_integrate            | 21.5 ms                                                | 19.6 ms: 1.09x faster                                                          |
| crypto_pyaes               | 76.7 ms                                                | 70.3 ms: 1.09x faster                                                          |
| regex_compile              | 141 ms                                                 | 130 ms: 1.09x faster                                                           |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.62 ms: 1.09x faster                                                          |
| tomli_loads                | 2.30 sec                                               | 2.12 sec: 1.09x faster                                                         |
| nqueens                    | 87.9 ms                                                | 80.9 ms: 1.09x faster                                                          |
| pickle_pure_python         | 320 us                                                 | 296 us: 1.08x faster                                                           |
| go                         | 149 ms                                                 | 138 ms: 1.08x faster                                                           |
| gc_traversal               | 4.01 ms                                                | 3.74 ms: 1.07x faster                                                          |
| deepcopy_memo              | 40.2 us                                                | 37.4 us: 1.07x faster                                                          |
| deepcopy                   | 365 us                                                 | 342 us: 1.07x faster                                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 702 ms: 1.07x faster                                                           |
| deepcopy_reduce            | 3.22 us                                                | 3.02 us: 1.06x faster                                                          |
| nbody                      | 96.0 ms                                                | 90.3 ms: 1.06x faster                                                          |
| scimark_monte_carlo        | 70.7 ms                                                | 66.6 ms: 1.06x faster                                                          |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 718 ms: 1.06x faster                                                           |
| sympy_expand               | 484 ms                                                 | 458 ms: 1.06x faster                                                           |
| xml_etree_parse            | 164 ms                                                 | 156 ms: 1.05x faster                                                           |
| pickle_dict                | 34.6 us                                                | 33.0 us: 1.05x faster                                                          |
| scimark_lu                 | 116 ms                                                 | 111 ms: 1.05x faster                                                           |
| richards                   | 49.8 ms                                                | 47.5 ms: 1.05x faster                                                          |
| sqlglot_normalize          | 113 ms                                                 | 108 ms: 1.04x faster                                                           |
| unpickle_list              | 5.21 us                                                | 5.02 us: 1.04x faster                                                          |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                           |
| tornado_http               | 98.1 ms                                                | 94.4 ms: 1.04x faster                                                          |
| pprint_pformat             | 1.55 sec                                               | 1.50 sec: 1.04x faster                                                         |
| json_loads                 | 29.2 us                                                | 28.2 us: 1.04x faster                                                          |
| fannkuch                   | 405 ms                                                 | 392 ms: 1.03x faster                                                           |
| xml_etree_iterparse        | 108 ms                                                 | 105 ms: 1.03x faster                                                           |
| docutils                   | 2.66 sec                                               | 2.59 sec: 1.03x faster                                                         |
| pprint_safe_repr           | 747 ms                                                 | 728 ms: 1.03x faster                                                           |
| pathlib                    | 18.5 ms                                                | 18.1 ms: 1.02x faster                                                          |
| pycparser                  | 1.19 sec                                               | 1.16 sec: 1.02x faster                                                         |
| sqlglot_optimize           | 55.3 ms                                                | 54.1 ms: 1.02x faster                                                          |
| json                       | 5.24 ms                                                | 5.14 ms: 1.02x faster                                                          |
| meteor_contest             | 109 ms                                                 | 107 ms: 1.02x faster                                                           |
| bench_thread_pool          | 834 us                                                 | 820 us: 1.02x faster                                                           |
| 2to3                       | 264 ms                                                 | 264 ms: 1.00x faster                                                           |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                           |
| scimark_fft                | 345 ms                                                 | 348 ms: 1.01x slower                                                           |
| spectral_norm              | 108 ms                                                 | 109 ms: 1.01x slower                                                           |
| dulwich_log                | 64.6 ms                                                | 65.7 ms: 1.02x slower                                                          |
| float                      | 78.9 ms                                                | 80.5 ms: 1.02x slower                                                          |
| xml_etree_process          | 56.9 ms                                                | 58.3 ms: 1.02x slower                                                          |
| unpack_sequence            | 43.5 ns                                                | 44.6 ns: 1.03x slower                                                          |
| chameleon                  | 6.70 ms                                                | 6.92 ms: 1.03x slower                                                          |
| regex_effbot               | 3.51 ms                                                | 3.64 ms: 1.04x slower                                                          |
| pickle                     | 11.0 us                                                | 11.4 us: 1.04x slower                                                          |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                                          |
| mako                       | 10.7 ms                                                | 11.2 ms: 1.05x slower                                                          |
| xml_etree_generate         | 81.1 ms                                                | 85.8 ms: 1.06x slower                                                          |
| scimark_sor                | 121 ms                                                 | 129 ms: 1.06x slower                                                           |
| regex_dna                  | 205 ms                                                 | 220 ms: 1.07x slower                                                           |
| pyflate                    | 434 ms                                                 | 467 ms: 1.08x slower                                                           |
| regex_v8                   | 22.9 ms                                                | 25.0 ms: 1.09x slower                                                          |
| sqlite_synth               | 2.57 us                                                | 2.82 us: 1.10x slower                                                          |
| pickle_list                | 4.59 us                                                | 5.04 us: 1.10x slower                                                          |
| unpickle                   | 13.8 us                                                | 15.4 us: 1.11x slower                                                          |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                          |
| coverage                   | 78.8 ms                                                | 94.2 ms: 1.20x slower                                                          |
| async_generators           | 374 ms                                                 | 450 ms: 1.20x slower                                                           |
| telco                      | 6.86 ms                                                | 8.37 ms: 1.22x slower                                                          |
| mypy2                      | 686 ms                                                 | 842 ms: 1.23x slower                                                           |
| python_startup_no_site     | 6.01 ms                                                | 8.77 ms: 1.46x slower                                                          |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                                   |

Benchmark hidden because not significant (2): dask, bench_mp_pool
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.98x