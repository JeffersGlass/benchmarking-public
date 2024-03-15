
# Results vs. 3.11.0

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: 1054202
- commit date: 2024-02-09
- overall geometric mean: 1.00x faster \*
- HPT reliability: 90.46%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 282 ms: 1.07x slower                                                           |
| chameleon      | 6.70 ms                                                | 7.40 ms: 1.11x slower                                                          |
| docutils       | 2.66 sec                                               | 2.71 sec: 1.02x slower                                                         |
| tornado_http   | 98.1 ms                                                | 98.6 ms: 1.01x slower                                                          |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 450 ms: 1.17x faster                                                           |
| async_tree_memoization     | 639 ms                                                 | 577 ms: 1.11x faster                                                           |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                         |
| async_tree_none_tg         | 491 ms                                                 | 459 ms: 1.07x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                         |
| async_tree_memoization_tg  | 626 ms                                                 | 593 ms: 1.06x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 733 ms: 1.04x faster                                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 725 ms: 1.03x faster                                                           |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                           |
| float          | 78.9 ms                                                | 91.4 ms: 1.16x slower                                                          |
| nbody          | 96.0 ms                                                | 121 ms: 1.26x slower                                                           |
| Geometric mean | (ref)                                                  | 1.12x slower                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 150 ms: 1.06x slower                                                           |
| regex_effbot   | 3.51 ms                                                | 3.77 ms: 1.07x slower                                                          |
| regex_v8       | 22.9 ms                                                | 25.1 ms: 1.10x slower                                                          |
| regex_dna      | 205 ms                                                 | 228 ms: 1.11x slower                                                           |
| Geometric mean | (ref)                                                  | 1.09x slower                                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                          |
| pickle_pure_python   | 320 us                                                 | 298 us: 1.07x faster                                                           |
| json_loads           | 29.2 us                                                | 27.7 us: 1.05x faster                                                          |
| unpickle_pure_python | 242 us                                                 | 232 us: 1.04x faster                                                           |
| unpickle_list        | 5.21 us                                                | 5.03 us: 1.04x faster                                                          |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                                           |
| pickle_dict          | 34.6 us                                                | 34.7 us: 1.00x slower                                                          |
| xml_etree_iterparse  | 108 ms                                                 | 109 ms: 1.01x slower                                                           |
| pickle               | 11.0 us                                                | 11.6 us: 1.06x slower                                                          |
| xml_etree_process    | 56.9 ms                                                | 60.6 ms: 1.06x slower                                                          |
| xml_etree_generate   | 81.1 ms                                                | 88.5 ms: 1.09x slower                                                          |
| unpickle             | 13.8 us                                                | 15.3 us: 1.10x slower                                                          |
| tomli_loads          | 2.30 sec                                               | 2.62 sec: 1.14x slower                                                         |
| pickle_list          | 4.59 us                                                | 5.25 us: 1.14x slower                                                          |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                          |
| python_startup_no_site | 6.01 ms                                                | 8.75 ms: 1.46x slower                                                          |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.9 ms: 1.30x slower                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 115 us: 4.53x faster                                                           |
| generators                 | 74.9 ms                                                | 29.4 ms: 2.55x faster                                                          |
| asyncio_tcp                | 875 ms                                                 | 492 ms: 1.78x faster                                                           |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.81 sec: 1.72x faster                                                         |
| json_dumps                 | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                          |
| coroutines                 | 27.0 ms                                                | 22.1 ms: 1.22x faster                                                          |
| async_tree_none            | 528 ms                                                 | 450 ms: 1.17x faster                                                           |
| deltablue                  | 3.92 ms                                                | 3.48 ms: 1.13x faster                                                          |
| richards_super             | 61.9 ms                                                | 55.7 ms: 1.11x faster                                                          |
| async_tree_memoization     | 639 ms                                                 | 577 ms: 1.11x faster                                                           |
| comprehensions             | 23.6 us                                                | 21.4 us: 1.10x faster                                                          |
| logging_silent             | 111 ns                                                 | 101 ns: 1.09x faster                                                           |
| gc_traversal               | 4.01 ms                                                | 3.71 ms: 1.08x faster                                                          |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                         |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.08x faster                                                          |
| pickle_pure_python         | 320 us                                                 | 298 us: 1.07x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 459 ms: 1.07x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                         |
| async_tree_memoization_tg  | 626 ms                                                 | 593 ms: 1.06x faster                                                           |
| mdp                        | 2.77 sec                                               | 2.64 sec: 1.05x faster                                                         |
| json_loads                 | 29.2 us                                                | 27.7 us: 1.05x faster                                                          |
| sqlglot_transpile          | 1.75 ms                                                | 1.67 ms: 1.05x faster                                                          |
| unpickle_pure_python       | 242 us                                                 | 232 us: 1.04x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 733 ms: 1.04x faster                                                           |
| raytrace                   | 309 ms                                                 | 298 ms: 1.04x faster                                                           |
| unpickle_list              | 5.21 us                                                | 5.03 us: 1.04x faster                                                          |
| sympy_sum                  | 169 ms                                                 | 163 ms: 1.03x faster                                                           |
| deepcopy                   | 365 us                                                 | 353 us: 1.03x faster                                                           |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 725 ms: 1.03x faster                                                           |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                           |
| logging_simple             | 6.22 us                                                | 6.03 us: 1.03x faster                                                          |
| json                       | 5.24 ms                                                | 5.11 ms: 1.03x faster                                                          |
| deepcopy_reduce            | 3.22 us                                                | 3.14 us: 1.02x faster                                                          |
| deepcopy_memo              | 40.2 us                                                | 39.7 us: 1.01x faster                                                          |
| richards                   | 49.8 ms                                                | 49.3 ms: 1.01x faster                                                          |
| sympy_str                  | 297 ms                                                 | 294 ms: 1.01x faster                                                           |
| pathlib                    | 18.5 ms                                                | 18.4 ms: 1.01x faster                                                          |
| sympy_integrate            | 21.5 ms                                                | 21.3 ms: 1.01x faster                                                          |
| scimark_lu                 | 116 ms                                                 | 116 ms: 1.01x faster                                                           |
| pickle_dict                | 34.6 us                                                | 34.7 us: 1.00x slower                                                          |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                           |
| tornado_http               | 98.1 ms                                                | 98.6 ms: 1.01x slower                                                          |
| xml_etree_iterparse        | 108 ms                                                 | 109 ms: 1.01x slower                                                           |
| bench_thread_pool          | 834 us                                                 | 846 us: 1.01x slower                                                           |
| dask                       | 365 ms                                                 | 370 ms: 1.01x slower                                                           |
| docutils                   | 2.66 sec                                               | 2.71 sec: 1.02x slower                                                         |
| chaos                      | 71.9 ms                                                | 73.2 ms: 1.02x slower                                                          |
| sympy_expand               | 484 ms                                                 | 494 ms: 1.02x slower                                                           |
| sqlglot_normalize          | 113 ms                                                 | 115 ms: 1.02x slower                                                           |
| create_gc_cycles           | 1.43 ms                                                | 1.48 ms: 1.03x slower                                                          |
| pycparser                  | 1.19 sec                                               | 1.23 sec: 1.04x slower                                                         |
| meteor_contest             | 109 ms                                                 | 113 ms: 1.04x slower                                                           |
| go                         | 149 ms                                                 | 156 ms: 1.05x slower                                                           |
| sqlglot_optimize           | 55.3 ms                                                | 58.4 ms: 1.06x slower                                                          |
| pickle                     | 11.0 us                                                | 11.6 us: 1.06x slower                                                          |
| regex_compile              | 141 ms                                                 | 150 ms: 1.06x slower                                                           |
| xml_etree_process          | 56.9 ms                                                | 60.6 ms: 1.06x slower                                                          |
| dulwich_log                | 64.6 ms                                                | 69.0 ms: 1.07x slower                                                          |
| pprint_pformat             | 1.55 sec                                               | 1.66 sec: 1.07x slower                                                         |
| 2to3                       | 264 ms                                                 | 282 ms: 1.07x slower                                                           |
| pprint_safe_repr           | 747 ms                                                 | 799 ms: 1.07x slower                                                           |
| regex_effbot               | 3.51 ms                                                | 3.77 ms: 1.07x slower                                                          |
| fannkuch                   | 405 ms                                                 | 440 ms: 1.09x slower                                                           |
| xml_etree_generate         | 81.1 ms                                                | 88.5 ms: 1.09x slower                                                          |
| regex_v8                   | 22.9 ms                                                | 25.1 ms: 1.10x slower                                                          |
| crypto_pyaes               | 76.7 ms                                                | 84.5 ms: 1.10x slower                                                          |
| unpickle                   | 13.8 us                                                | 15.3 us: 1.10x slower                                                          |
| chameleon                  | 6.70 ms                                                | 7.40 ms: 1.11x slower                                                          |
| nqueens                    | 87.9 ms                                                | 97.6 ms: 1.11x slower                                                          |
| regex_dna                  | 205 ms                                                 | 228 ms: 1.11x slower                                                           |
| sqlite_synth               | 2.57 us                                                | 2.88 us: 1.12x slower                                                          |
| tomli_loads                | 2.30 sec                                               | 2.62 sec: 1.14x slower                                                         |
| pickle_list                | 4.59 us                                                | 5.25 us: 1.14x slower                                                          |
| scimark_monte_carlo        | 70.7 ms                                                | 81.1 ms: 1.15x slower                                                          |
| float                      | 78.9 ms                                                | 91.4 ms: 1.16x slower                                                          |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                          |
| async_generators           | 374 ms                                                 | 449 ms: 1.20x slower                                                           |
| coverage                   | 78.8 ms                                                | 94.8 ms: 1.20x slower                                                          |
| pyflate                    | 434 ms                                                 | 526 ms: 1.21x slower                                                           |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.11 ms: 1.22x slower                                                          |
| hexiom                     | 6.89 ms                                                | 8.44 ms: 1.22x slower                                                          |
| nbody                      | 96.0 ms                                                | 121 ms: 1.26x slower                                                           |
| telco                      | 6.86 ms                                                | 8.65 ms: 1.26x slower                                                          |
| mypy2                      | 686 ms                                                 | 873 ms: 1.27x slower                                                           |
| scimark_fft                | 345 ms                                                 | 440 ms: 1.27x slower                                                           |
| mako                       | 10.7 ms                                                | 13.9 ms: 1.30x slower                                                          |
| unpack_sequence            | 43.5 ns                                                | 57.1 ns: 1.31x slower                                                          |
| spectral_norm              | 108 ms                                                 | 144 ms: 1.33x slower                                                           |
| python_startup_no_site     | 6.01 ms                                                | 8.75 ms: 1.46x slower                                                          |
| Geometric mean             | (ref)                                                  | 1.00x faster                                                                   |

Benchmark hidden because not significant (3): logging_format, scimark_sor, bench_mp_pool
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 90.46% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x