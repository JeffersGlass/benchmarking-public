
# Results vs. 3.11.0

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: 7b9e10f
- commit date: 2024-02-08
- overall geometric mean: 1.01x faster \*
- HPT reliability: 84.73%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 282 ms: 1.07x slower                                                           |
| chameleon      | 6.70 ms                                                | 7.18 ms: 1.07x slower                                                          |
| docutils       | 2.66 sec                                               | 2.69 sec: 1.01x slower                                                         |
| tornado_http   | 98.1 ms                                                | 98.7 ms: 1.01x slower                                                          |
| Geometric mean | (ref)                                                  | 1.04x slower                                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 448 ms: 1.18x faster                                                           |
| async_tree_memoization     | 639 ms                                                 | 574 ms: 1.11x faster                                                           |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                         |
| async_tree_none_tg         | 491 ms                                                 | 456 ms: 1.08x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                         |
| async_tree_memoization_tg  | 626 ms                                                 | 595 ms: 1.05x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 731 ms: 1.04x faster                                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 721 ms: 1.04x faster                                                           |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                           |
| float          | 78.9 ms                                                | 88.5 ms: 1.12x slower                                                          |
| nbody          | 96.0 ms                                                | 115 ms: 1.20x slower                                                           |
| Geometric mean | (ref)                                                  | 1.09x slower                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.65 ms: 1.04x slower                                                          |
| regex_compile  | 141 ms                                                 | 148 ms: 1.05x slower                                                           |
| regex_dna      | 205 ms                                                 | 222 ms: 1.09x slower                                                           |
| regex_v8       | 22.9 ms                                                | 25.0 ms: 1.09x slower                                                          |
| Geometric mean | (ref)                                                  | 1.07x slower                                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                          |
| pickle_pure_python   | 320 us                                                 | 298 us: 1.07x faster                                                           |
| json_loads           | 29.2 us                                                | 27.7 us: 1.06x faster                                                          |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.05x faster                                                           |
| unpickle_pure_python | 242 us                                                 | 231 us: 1.05x faster                                                           |
| unpickle_list        | 5.21 us                                                | 4.99 us: 1.04x faster                                                          |
| pickle_dict          | 34.6 us                                                | 35.3 us: 1.02x slower                                                          |
| xml_etree_process    | 56.9 ms                                                | 59.9 ms: 1.05x slower                                                          |
| pickle               | 11.0 us                                                | 11.9 us: 1.08x slower                                                          |
| xml_etree_generate   | 81.1 ms                                                | 88.1 ms: 1.09x slower                                                          |
| tomli_loads          | 2.30 sec                                               | 2.54 sec: 1.10x slower                                                         |
| unpickle             | 13.8 us                                                | 15.3 us: 1.11x slower                                                          |
| pickle_list          | 4.59 us                                                | 5.28 us: 1.15x slower                                                          |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                                   |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                          |
| python_startup_no_site | 6.01 ms                                                | 8.83 ms: 1.47x slower                                                          |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.2 ms: 1.24x slower                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 114 us: 4.55x faster                                                           |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.56x faster                                                          |
| asyncio_tcp                | 875 ms                                                 | 488 ms: 1.79x faster                                                           |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.72x faster                                                         |
| json_dumps                 | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                          |
| coroutines                 | 27.0 ms                                                | 22.1 ms: 1.22x faster                                                          |
| async_tree_none            | 528 ms                                                 | 448 ms: 1.18x faster                                                           |
| comprehensions             | 23.6 us                                                | 20.5 us: 1.15x faster                                                          |
| gc_traversal               | 4.01 ms                                                | 3.49 ms: 1.15x faster                                                          |
| richards_super             | 61.9 ms                                                | 54.3 ms: 1.14x faster                                                          |
| deltablue                  | 3.92 ms                                                | 3.51 ms: 1.12x faster                                                          |
| async_tree_memoization     | 639 ms                                                 | 574 ms: 1.11x faster                                                           |
| unpack_sequence            | 43.5 ns                                                | 39.9 ns: 1.09x faster                                                          |
| logging_silent             | 111 ns                                                 | 102 ns: 1.09x faster                                                           |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                         |
| async_tree_none_tg         | 491 ms                                                 | 456 ms: 1.08x faster                                                           |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.07x faster                                                          |
| pickle_pure_python         | 320 us                                                 | 298 us: 1.07x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                         |
| mdp                        | 2.77 sec                                               | 2.62 sec: 1.06x faster                                                         |
| json_loads                 | 29.2 us                                                | 27.7 us: 1.06x faster                                                          |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.05x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 595 ms: 1.05x faster                                                           |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.05x faster                                                           |
| sqlglot_transpile          | 1.75 ms                                                | 1.67 ms: 1.05x faster                                                          |
| unpickle_pure_python       | 242 us                                                 | 231 us: 1.05x faster                                                           |
| raytrace                   | 309 ms                                                 | 295 ms: 1.04x faster                                                           |
| unpickle_list              | 5.21 us                                                | 4.99 us: 1.04x faster                                                          |
| logging_simple             | 6.22 us                                                | 5.96 us: 1.04x faster                                                          |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 731 ms: 1.04x faster                                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 721 ms: 1.04x faster                                                           |
| deepcopy_reduce            | 3.22 us                                                | 3.11 us: 1.03x faster                                                          |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                           |
| deepcopy                   | 365 us                                                 | 354 us: 1.03x faster                                                           |
| richards                   | 49.8 ms                                                | 48.3 ms: 1.03x faster                                                          |
| sympy_integrate            | 21.5 ms                                                | 21.0 ms: 1.02x faster                                                          |
| chaos                      | 71.9 ms                                                | 70.6 ms: 1.02x faster                                                          |
| json                       | 5.24 ms                                                | 5.16 ms: 1.02x faster                                                          |
| pathlib                    | 18.5 ms                                                | 18.3 ms: 1.01x faster                                                          |
| scimark_lu                 | 116 ms                                                 | 115 ms: 1.01x faster                                                           |
| sympy_str                  | 297 ms                                                 | 294 ms: 1.01x faster                                                           |
| deepcopy_memo              | 40.2 us                                                | 39.7 us: 1.01x faster                                                          |
| logging_format             | 6.81 us                                                | 6.76 us: 1.01x faster                                                          |
| tornado_http               | 98.1 ms                                                | 98.7 ms: 1.01x slower                                                          |
| bench_thread_pool          | 834 us                                                 | 842 us: 1.01x slower                                                           |
| scimark_sor                | 121 ms                                                 | 123 ms: 1.01x slower                                                           |
| docutils                   | 2.66 sec                                               | 2.69 sec: 1.01x slower                                                         |
| create_gc_cycles           | 1.43 ms                                                | 1.46 ms: 1.02x slower                                                          |
| sympy_expand               | 484 ms                                                 | 495 ms: 1.02x slower                                                           |
| pickle_dict                | 34.6 us                                                | 35.3 us: 1.02x slower                                                          |
| sqlglot_normalize          | 113 ms                                                 | 116 ms: 1.03x slower                                                           |
| meteor_contest             | 109 ms                                                 | 113 ms: 1.04x slower                                                           |
| regex_effbot               | 3.51 ms                                                | 3.65 ms: 1.04x slower                                                          |
| sqlglot_optimize           | 55.3 ms                                                | 58.0 ms: 1.05x slower                                                          |
| regex_compile              | 141 ms                                                 | 148 ms: 1.05x slower                                                           |
| pprint_pformat             | 1.55 sec                                               | 1.64 sec: 1.05x slower                                                         |
| xml_etree_process          | 56.9 ms                                                | 59.9 ms: 1.05x slower                                                          |
| pycparser                  | 1.19 sec                                               | 1.25 sec: 1.06x slower                                                         |
| pprint_safe_repr           | 747 ms                                                 | 790 ms: 1.06x slower                                                           |
| nqueens                    | 87.9 ms                                                | 93.5 ms: 1.06x slower                                                          |
| 2to3                       | 264 ms                                                 | 282 ms: 1.07x slower                                                           |
| crypto_pyaes               | 76.7 ms                                                | 82.0 ms: 1.07x slower                                                          |
| fannkuch                   | 405 ms                                                 | 433 ms: 1.07x slower                                                           |
| chameleon                  | 6.70 ms                                                | 7.18 ms: 1.07x slower                                                          |
| dulwich_log                | 64.6 ms                                                | 69.4 ms: 1.07x slower                                                          |
| pickle                     | 11.0 us                                                | 11.9 us: 1.08x slower                                                          |
| regex_dna                  | 205 ms                                                 | 222 ms: 1.09x slower                                                           |
| xml_etree_generate         | 81.1 ms                                                | 88.1 ms: 1.09x slower                                                          |
| regex_v8                   | 22.9 ms                                                | 25.0 ms: 1.09x slower                                                          |
| scimark_monte_carlo        | 70.7 ms                                                | 77.6 ms: 1.10x slower                                                          |
| tomli_loads                | 2.30 sec                                               | 2.54 sec: 1.10x slower                                                         |
| unpickle                   | 13.8 us                                                | 15.3 us: 1.11x slower                                                          |
| sqlite_synth               | 2.57 us                                                | 2.86 us: 1.11x slower                                                          |
| float                      | 78.9 ms                                                | 88.5 ms: 1.12x slower                                                          |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.75 ms: 1.14x slower                                                          |
| pickle_list                | 4.59 us                                                | 5.28 us: 1.15x slower                                                          |
| go                         | 149 ms                                                 | 172 ms: 1.16x slower                                                           |
| pyflate                    | 434 ms                                                 | 504 ms: 1.16x slower                                                           |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                          |
| hexiom                     | 6.89 ms                                                | 8.21 ms: 1.19x slower                                                          |
| nbody                      | 96.0 ms                                                | 115 ms: 1.20x slower                                                           |
| coverage                   | 78.8 ms                                                | 94.7 ms: 1.20x slower                                                          |
| scimark_fft                | 345 ms                                                 | 425 ms: 1.23x slower                                                           |
| async_generators           | 374 ms                                                 | 460 ms: 1.23x slower                                                           |
| mako                       | 10.7 ms                                                | 13.2 ms: 1.24x slower                                                          |
| spectral_norm              | 108 ms                                                 | 137 ms: 1.27x slower                                                           |
| mypy2                      | 686 ms                                                 | 872 ms: 1.27x slower                                                           |
| telco                      | 6.86 ms                                                | 8.76 ms: 1.28x slower                                                          |
| python_startup_no_site     | 6.01 ms                                                | 8.83 ms: 1.47x slower                                                          |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                                   |

Benchmark hidden because not significant (4): bench_mp_pool, asyncio_websockets, xml_etree_iterparse, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 84.73% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x